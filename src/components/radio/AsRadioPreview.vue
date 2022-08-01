<template>
  <div class="as-mt-24">
    <AsRadio
      id="radio-1"
      name="as-radio"
      checked
      for="radio-1"
      label="Cheked"
    />

    <AsRadio id="radio-2" name="as-radio" for="radio-2" label="Uncheked" />

    <AsRadio
      id="radio-3"
      name="as-radio"
      disabled
      for="radio-3"
      label="Disabled"
    />
  </div>
</template>

<script setup>
import AsRadio from "./AsRadio.vue";
</script>
