<template>
  <p class="as-color-secondary as-mb-16">
    Use the <code>.as-input, .as-input__search</code> classes
  </p>
  <div class="col-md-6 as-mb-24">
    <AsInput
      search
      type="text"
      data-lpignore="true"
      placeholder="Default Search"
    />
  </div>

  <div class="col-md-6 as-mb-24">
    <AsInput
      search
      type="text"
      data-lpignore="true"
      placeholder="Search with caption"
    />
    <span id="searchCaption" class="as-info as-info--secondary as-mt-4">
      Caption here
    </span>
  </div>

  <p class="as-color-secondary as-mb-16">
    Use the
    <code>.as-input, .as-input--disable, .as-input__search</code> classes
  </p>
  <div class="col-md-6 as-mb-24">
    <AsInput
      search
      type="text"
      data-lpignore="true"
      placeholder="Search disabled state"
      disabled
    />
  </div>
</template>

<script setup>
import AsInput from "./AsInput.vue";
</script>
