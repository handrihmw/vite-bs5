<template>
  <div class="as-accordion">
    <slot />
  </div>
</template>

<script setup>
import { inject, onMounted, ref, provide } from "vue";

let AccordionIndex = ref(false);
const AccordionStatus = inject("AccordionStatus");

const visible = () => {
  return AccordionIndex == AccordionStatus.active;
};

provide("visible", visible);

const toggleAccordion = () => {
  if (visible()) {
    AccordionStatus.active = null;
  } else {
    AccordionStatus.active = AccordionIndex;
  }
};

provide("toggleAccordion", toggleAccordion);

onMounted(() => {
  AccordionIndex = AccordionStatus.count++;
});
</script>

<style lang="scss">
@use "@/assets/scss/components/accordion";
</style>
