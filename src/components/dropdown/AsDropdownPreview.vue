<template>
  <p class="as-color-secondary as-mb-16">
    Use the <code>.as-dropdown, .as-dropdown__menu</code> classes
  </p>
  <div class="col-md-6 as-mb-24">
    <AsDropdown />
  </div>

  <div class="col-md-6 as-mb-24">
    <label for="dropdown" class="as-text-16-semibold as-mb-8"
      >Input Label</label
    >
    <AsDropdown />
    <span id="dropdownCaption" class="as-info as-info--secondary as-mt-4">
      Caption here
    </span>
  </div>

  <p class="as-color-secondary as-mb-16">
    Use the
    <code>.as-dropdown, .as-dropdown--sm, .as-dropdown__menu</code> classes
  </p>
  <AsDropdown sm />

  <p class="as-color-secondary as-mb-16 as-mt-24">
    Use the
    <code>.as-dropdown, .as-dropdown--disable, .as-dropdown__menu</code> classes
  </p>
  <div class="col-md-6">
    <AsDropdown disabled />
  </div>
</template>

<script setup>
import AsDropdown from "./AsDropdown.vue";
</script>

<style></style>
