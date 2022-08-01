<template>
  <a :href="path" :class="className" role="link">
    <slot />
  </a>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  danger: Boolean,
  disabled: Boolean,
  sm: Boolean,
  md: Boolean,
  lg: Boolean,
  withIcon: Boolean,

  path: {
    default: "#",
    type: String,
  },
});

const className = computed(() => {
  let baseName = "as-link";

  return {
    [baseName]: true,
    [`${baseName}--danger`]: props.danger && !props.disabled,
    [`${baseName}--disabled`]: props.disabled,
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--md`]: props.md,
    [`${baseName}--lg`]: props.lg,
    "as-link-icon": props.withIcon,
  };
});
</script>

<style lang="scss" scoped>
@use "@/assets/scss/components/link.scss";
</style>
