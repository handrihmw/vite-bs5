<template>
  <div class="as-input__group">
    <slot />
  </div>
</template>

<script setup>
const props = defineProps({
  groupPrefix: String,
  placeholder: String,
  required: Boolean,
});
</script>

<style lang="scss">
@use "@/assets/scss/components/input.scss";
</style>
