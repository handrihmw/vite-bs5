<template>
  <div class="row">
    <div class="col-md-4 as-mb-16">
      <label for="progressBar" class="as-text-16-semibold as-mb-8"
        >with <code>valuenow</code> 20</label
      >
      <AsProgress>
        <AsProgressBar
          valuenow="20"
          valuemin="0"
          valuemax="100"
        ></AsProgressBar>
      </AsProgress>
    </div>
    <div class="col-md-4 as-mb-16">
      <label for="progressBar" class="as-text-16-semibold as-mb-8"
        >with <code>valuenow</code> 40</label
      >
      <AsProgress>
        <AsProgressBar
          valuenow="40"
          valuemin="0"
          valuemax="100"
        ></AsProgressBar>
      </AsProgress>
    </div>
    <div class="col-md-4 as-mb-16">
      <label for="progressBar" class="as-text-16-semibold as-mb-8"
        >with <code>valuenow</code> 90</label
      >
      <AsProgress>
        <AsProgressBar
          valuenow="90"
          valuemin="0"
          valuemax="100"
        ></AsProgressBar>
      </AsProgress>
    </div>
  </div>
</template>

<script setup>
import AsProgress from "./AsProgress.vue";
import AsProgressBar from "./AsProgressBar.vue";
</script>
