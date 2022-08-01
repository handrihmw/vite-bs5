<template>
  <a :class="className" role="button" v-if="anchor">
    <slot />
  </a>
  <button :class="className" v-else>
    <slot />
  </button>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  active: Boolean,
  anchor: Boolean,
  danger: Boolean,
  dark: Boolean,
  fluid: Boolean,
  primary: Boolean,
  secondary: Boolean,
  success: Boolean,
  disabled: Boolean,
  noBorder: Boolean,
  sm: Boolean,
  md: Boolean,
  lg: Boolean,
  withIcon: Boolean,
});

const className = computed(() => {
  let baseName = "as-btn";

  return {
    [baseName]: true,
    [`${baseName}--active`]: props.active,
    [`${baseName}--danger`]: props.danger && !props.disabled,
    [`${baseName}--dark`]: props.dark && !props.disabled,
    [`${baseName}--fluid`]: props.fluid,
    [`${baseName}--primary`]: props.primary && !props.disabled,
    [`${baseName}--secondary`]: props.secondary && !props.disabled,
    [`${baseName}--success`]: props.success && !props.disabled,
    [`${baseName}--disabled`]: props.disabled,
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--md`]: props.md,
    [`${baseName}--lg`]: props.lg,
    "as-btn-icon": props.withIcon,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/button.scss";
@use "@/assets/scss/components/button-icon.scss";
</style>
