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
  anchor: Boolean,
  danger: Boolean,
  link: Boolean,
  disabled: Boolean,
  fluid: Boolean,
  xs: Boolean,
  sm: Boolean,
  md: Boolean,
  lg: Boolean,
});

const className = computed(() => {
  let baseName = "as-btn-text";

  return {
    [baseName]: true,
    [`${baseName}--danger`]: props.danger,
    [`${baseName}--link`]: props.link,
    [`${baseName}--disabled`]: props.disabled,
    [`${baseName}--fluid`]: props.fluid,
    [`${baseName}--xs`]: props.xs,
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--md`]: props.md,
    [`${baseName}--lg`]: props.lg,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/button-text.scss";
</style>
