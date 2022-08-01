<template>
  <div :class="className">
    <slot />
  </div>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  noLeft: Boolean,
  noRight: Boolean,
  left: Boolean,
  right: Boolean,
});

const className = computed(() => {
  let baseName = "as-input__group-text";

  return {
    [baseName]: true,
    [`as-border-radius-no-left`]: props.noLeft,
    [`as-border-radius-no-right`]: props.noRight,
    [`${baseName}--left`]: props.left,
    [`${baseName}--right`]: props.right,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/input.scss";
</style>
