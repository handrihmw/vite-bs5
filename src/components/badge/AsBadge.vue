<template>
  <span :class="className">
    <slot />
  </span>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  active: Boolean,
  black: Boolean,
  blue: Boolean,
  light: Boolean,
  soft: Boolean,
  orange: Boolean,
  yellow: Boolean,
  green: Boolean,
  red: Boolean,
  rounded: Boolean,
  icon: Boolean,
  sm: Boolean,
  md: Boolean,
  lg: Boolean,
  disabled: Boolean,
});

const className = computed(() => {
  let baseName = "as-badge";

  return {
    [baseName]: true,
    [`${baseName}--active`]: props.active,
    [`${baseName}--black`]: props.black && !props.disabled,
    [`${baseName}--blue`]: props.blue && !props.disabled,
    [`${baseName}--fluid`]: props.fluid,
    [`${baseName}--light`]: props.light && !props.disabled,
    [`${baseName}--soft`]: props.soft && !props.disabled,
    [`${baseName}--orange`]: props.orange && !props.disabled,
    [`${baseName}--yellow`]: props.yellow && !props.disabled,
    [`${baseName}--green`]: props.green && !props.disabled,
    [`${baseName}--red`]: props.red && !props.disabled,
    [`${baseName}--rounded`]: props.rounded && !props.disabled,
    [`${baseName}--icon`]: props.icon,

    [`${baseName}--sm`]: props.sm,
    [`${baseName}--md`]: props.md,
    [`${baseName}--lg`]: props.lg,
    [`${baseName}--disabled`]: props.disabled,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/badge.scss";
</style>
