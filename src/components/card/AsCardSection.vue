<template>
  <div :class="className">
    <slot />
  </div>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  md: Boolean,
  lg: Boolean,
  flex: Boolean,
  center: Boolean,
  top: Boolean,
  bottom: Boolean,
  left: Boolean,
});

const className = computed(() => {
  let baseName = "as-card__section";

  return {
    [baseName]: true,
    [`${baseName}--md`]: props.md,
    [`${baseName}--lg`]: props.lg,
    [`${baseName}--flex`]: props.flex,
    [`${baseName}--center`]: props.center,
    [`${baseName}--top`]: props.top,
    [`${baseName}--bottom`]: props.bottom,
    [`${baseName}--left`]: props.left,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/card.scss";
</style>
