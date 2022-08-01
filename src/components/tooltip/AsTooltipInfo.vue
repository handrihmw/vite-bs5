<template>
  <span :class="className" class="as-tooltip__info">
    {{ text }}
  </span>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  sm: Boolean,
  md: Boolean,
  bottom: Boolean,
  top: Boolean,
  left: Boolean,
  right: Boolean,
  text: {
    default:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa, officia praesentium laudantium in fugiat excepturi.",
    type: String,
  },
});

const className = computed(() => {
  let baseName = "as-tooltip__info";
  return {
    [baseName]: true,
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--md`]: props.md,
    [`${baseName}--bottom`]: props.bottom,
    [`${baseName}--top`]: props.top,
    [`${baseName}--left`]: props.left,
    [`${baseName}--right`]: props.right,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/tooltip.scss";
</style>
