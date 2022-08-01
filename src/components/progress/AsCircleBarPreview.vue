<template>
  <div class="row">
    <div class="col-md-4">
      <label for="progressBar" class="as-text-16-semibold as-mb-8"
        >with <code>valuenow</code> 20</label
      >
      <AsCircleBar valueNow="10"></AsCircleBar>
    </div>
    <div class="col-md-4">
      <label for="progressBar" class="as-text-16-semibold as-mb-8"
        >with <code>valuenow</code> 60</label
      >
      <AsCircleBar valueNow="60"></AsCircleBar>
    </div>
    <div class="col-md-4">
      <label for="progressBar" class="as-text-16-semibold as-mb-8"
        >with <code>valuenow</code> 90</label
      >
      <AsCircleBar valueNow="90"></AsCircleBar>
    </div>
  </div>
</template>

<script setup>
import AsCircleBar from "./AsCircleBar.vue";
</script>
