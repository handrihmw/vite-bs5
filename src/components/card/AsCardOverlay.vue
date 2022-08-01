<template>
  <div :class="className">
    <slot />
  </div>
</template>

<script setup>
import { computed } from "vue";

const className = computed(() => {
  let baseName = "as-card__overlay";
});
</script>

<style lang="scss">
@use "@/assets/scss/components/card.scss";
</style>
