<template>
  <div class="as-banner">
    <img class="as-banner__image" :src="src" />
    <div class="as-banner__body">
      <slot />
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  src: {
    required: true,
    type: String,
  },
});
</script>

<style lang="scss">
@use "@/assets/scss/components/banner";
</style>
