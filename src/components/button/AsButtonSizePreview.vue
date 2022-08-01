<template>
  <div class="d-flex flex-wrap gap-3 as-mt-16">
    <AsButton primary sm>Small</AsButton>
    <AsButton primary>Medium</AsButton>
    <AsButton primary lg>Large</AsButton>
  </div>

  <div class="d-flex flex-wrap gap-3 as-mt-24">
    <AsButtonOutline primary sm>Small</AsButtonOutline>
    <AsButtonOutline primary>Medium</AsButtonOutline>
    <AsButtonOutline primary lg>Large</AsButtonOutline>
  </div>
</template>

<script setup>
import AsButton from "./AsButton.vue";
import AsButtonOutline from "./AsButtonOutline.vue";
</script>
