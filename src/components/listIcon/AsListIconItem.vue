<template>
  <li :class="className">
    <span>{{ text }}</span>
  </li>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  sm: Boolean,
  md: Boolean,
  lg: Boolean,
  xlg: Boolean,
  white: Boolean,
  text: {
    default: "List icon item ",
    type: String,
  },
});

const className = computed(() => {
  let baseName = "as-list-icon__item";

  return {
    [baseName]: true,
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--md`]: props.md,
    [`${baseName}--lg`]: props.lg,
    [`${baseName}--xlg`]: props.xlg,
    [`${baseName}--white`]: props.white,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/list-icon.scss";
</style>
