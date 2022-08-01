<template>
  <img
    :class="className"
    src="https://source.unsplash.com/1600x900/?nature,water"
    alt="rover"
  />
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  top: Boolean,
  theme: Boolean,
  purchased: Boolean,
  installed: Boolean,
});

const className = computed(() => {
  let baseName = "as-card__image";

  return {
    [baseName]: true,
    [`${baseName}--top`]: props.top,
    [`${baseName}--theme`]: props.theme,
    [`${baseName}--purchased`]: props.purchased,
    [`${baseName}--installed`]: props.installed,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/card.scss";
</style>
