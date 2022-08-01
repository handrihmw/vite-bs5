<template>
  <div class="d-flex flex-wrap gap-3 as-mt-16">
    <AsButton primary withIcon
      ><i class="as-icon-arrow-left"></i><span>Icon Left</span></AsButton
    >
    <AsButton primary withIcon
      ><span>Icon Right </span><i class="as-icon-arrow-right"></i
    ></AsButton>
  </div>
  <div class="d-flex flex-wrap gap-3 as-mt-24">
    <AsButtonOutline primary withIcon
      ><i class="as-icon-arrow-left"></i><span>Icon Left</span></AsButtonOutline
    >
    <AsButtonOutline primary withIcon
      ><span>Icon Right </span><i class="as-icon-arrow-right"></i
    ></AsButtonOutline>
  </div>
</template>

<script setup>
import AsButton from "./AsButton.vue";
import AsButtonOutline from "./AsButtonOutline.vue";
</script>
