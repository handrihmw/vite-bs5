<template>
  <div
    @click="toggleAccordion"
    class="as-accordion-soft__header"
    :class="{ 'as-accordion-soft__header--open': visible() }"
  >
    <slot />
    <i
      class="as-icon-blue"
      :class="{
        'as-icon-minus': visible(),
        'as-icon-plus': !visible(),
      }"
    ></i>
  </div>
</template>

<script setup>
import { inject } from "vue";

const visible = inject("visible");
const toggleAccordion = inject("toggleAccordion");
</script>
