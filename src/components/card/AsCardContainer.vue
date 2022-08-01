<template>
  <div :class="className">
    <slot />
  </div>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  thumb: Boolean,
  flex: Boolean,
  border: Boolean,
  xsm: Boolean,
  sm: Boolean,
  md: Boolean,
  lg: Boolean,
  xlg: Boolean,
  fullCol: Boolean,
  service: Boolean,
});

const className = computed(() => {
  let baseName = "as-card__container";

  return {
    [baseName]: true,
    [`${baseName}--thumb`]: props.thumb,
    [`${baseName}--flex`]: props.flex,
    [`${baseName}--border`]: props.border,
    [`${baseName}--xsm`]: props.xsm,
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--md`]: props.md,
    [`${baseName}--lg`]: props.lg,
    [`${baseName}--xlg`]: props.xlg,
    [`${baseName}--full-col`]: props.fullCol,
    [`${baseName}--service`]: props.service,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/card.scss";
</style>
