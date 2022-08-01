<template>
  <p class="as-color-secondary as-mb-16">
    Use <code>.as-input, .as-input__select</code> classes
  </p>
  <div class="col-md-6 as-mb-24">
    <AsInputSelect> </AsInputSelect>
  </div>

  <div class="col-md-6 as-mb-24">
    <label for="selectInput" class="as-text-16-semibold as-mb-8"
      >Select label</label
    >
    <AsInputSelect> </AsInputSelect>
    <span id="selectInput" class="as-info as-info--secondary as-mb-8">
      Caption here
    </span>
  </div>

  <p class="as-color-secondary as-mb-16">
    Use <code>.as-input, .as-input__select, .as-input__select--sm</code> classes
  </p>
  <div class="col-md-12">
    <AsInputSelect sm> </AsInputSelect>
  </div>
</template>

<script setup>
import AsInputSelect from "./AsInputSelect.vue";
</script>
