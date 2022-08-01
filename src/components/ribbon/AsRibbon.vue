<template>
  <span :class="className">{{ label }}</span>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  green: Boolean,
  red: Boolean,
  label: {
    default: "Label",
    type: String,
  },
});

const className = computed(() => {
  let baseName = "as-ribbon";
  return {
    [baseName]: true,
    [`${baseName}--green`]: props.green,
    [`${baseName}--red`]: props.red,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/ribbon.scss";
</style>
