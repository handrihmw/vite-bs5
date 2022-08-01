<template>
  <div :class="className">
    <slot />
  </div>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  cpanel: Boolean,
  ssl: Boolean,
  cms: Boolean,
  xray: Boolean,
  full: Boolean,
});

const className = computed(() => {
  let baseName = "as-card--background";

  return {
    [baseName]: true,
    [`${baseName}-cpanel`]: props.cpanel,
    [`${baseName}-ssl`]: props.ssl,
    [`${baseName}-cms`]: props.cms,
    [`${baseName}-xray`]: props.xray,
    [`${baseName}-full`]: props.full,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/card.scss";
</style>
