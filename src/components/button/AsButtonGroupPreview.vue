<template>
  <AsButtonGroup class="as-mt-16">
    <AsButton primary>Button 1</AsButton>
    <AsButton primary>Button 2</AsButton>
    <AsButton primary>Button 3</AsButton>
  </AsButtonGroup>

  <AsButtonGroup class="as-mt-24">
    <AsButtonOutline primary>Button 1</AsButtonOutline>
    <AsButtonOutline primary>Button 2</AsButtonOutline>
    <AsButtonOutline primary>Button 3</AsButtonOutline>
  </AsButtonGroup>

  <AsButtonGroup class="as-mt-24">
    <AsButtonOutline><i class="as-icon-grid"></i></AsButtonOutline>
    <AsButtonOutline><i class="as-icon-filter"></i></AsButtonOutline>
    <AsButtonOutline><i class="as-icon-list"></i></AsButtonOutline>
  </AsButtonGroup>
</template>

<script setup>
import AsButtonGroup from "./AsButtonGroup.vue";
import AsButton from "./AsButton.vue";
import AsButtonOutline from "./AsButtonOutline.vue";
</script>
