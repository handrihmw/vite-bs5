<template>
  <div
    @click="toggleAccordion"
    class="as-accordion__header"
    :class="{ 'as-accordion__header--open': visible() }"
  >
    <div class="d-flex w-100 align-items-center justify-content-between">
      <slot />
      <div class="icon-container d-flex align-items-center gap-4">
        <AsBadge class="label-desktop" v-if="withLabel" light>{{
          textLabel
        }}</AsBadge>
        <i
          class="as-icon-blue"
          :class="{
            'as-icon-arrow-top': visible(),
            'as-icon-arrow-down': !visible(),
          }"
        ></i>
      </div>
    </div>
    <AsBadge class="label-mobile as-mt-8" v-if="withLabel" light>{{
      textLabel
    }}</AsBadge>
  </div>
</template>

<script setup>
import { inject } from "vue";
import AsBadge from "../badge/AsBadge.vue";

const visible = inject("visible");
const toggleAccordion = inject("toggleAccordion");

const props = defineProps({
  withLabel: Boolean,
  textLabel: {
    default: "Label",
    type: String,
  },
});
</script>
