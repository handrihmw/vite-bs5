<template>
  <p class="as-color-secondary as-mb-16">
    Use the
    <code>.as-dropdown, .as-dropdown--left, .as-dropdown__menu</code>
    classes
  </p>
  <div class="col-md-6 as-mb-24">
    <AsDropdown left />
  </div>

  <p class="as-color-secondary as-mb-16">
    Use the
    <code>.as-dropdown, .as-dropdown--right, .as-dropdown__menu</code>
    classes
  </p>
  <div class="col-md-6 as-mb-24">
    <AsDropdown right />
  </div>

  <p class="as-color-secondary as-mb-16">
    Use the
    <code
      >.as-dropdown, .as-dropdown--left, .as-dropdown--sm,
      .as-dropdown__menu</code
    >
    classes
  </p>
  <div class="col-md-6 as-mb-24">
    <AsDropdown sm left />
  </div>

  <p class="as-color-secondary as-mb-16">
    Use the
    <code
      >.as-dropdown, .as-dropdown--left, .as-dropdown--disable,
      .as-dropdown__menu</code
    >
    classes
  </p>
  <div class="col-md-6 as-mb-24">
    <AsDropdown disabled left />
  </div>
</template>

<script setup>
import AsDropdown from "./AsDropdown.vue";
</script>

<style></style>
