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
  disabled: Boolean,
  sm: Boolean,
  md: Boolean,
  lg: Boolean,
  withIcon: Boolean,
});

const className = computed(() => {
  let baseName = "as-btn-filter";

  return {
    [baseName]: true,
    [`${baseName}--active`]: props.active,
    [`${baseName}--disabled`]: props.disabled,
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--md`]: props.md,
    [`${baseName}--lg`]: props.lg,
    "as-btn-icon": props.withIcon,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/button-filter.scss";
</style>
