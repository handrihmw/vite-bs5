<template>
  <div :class="className">
    <slot />
  </div>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  sm: Boolean,
  md: Boolean,
  service: Boolean,
});

const className = computed(() => {
  let baseName = "as-card__header";

  return {
    [baseName]: true,
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--md`]: props.md,
    [`${baseName}--service`]: props.service,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/card.scss";
</style>
