<template>
  <div class="d-flex gap-5 as-mt-16 align-items-center">
    <AsLink sm>Small</AsLink>
    <AsLink>Medium</AsLink>
    <AsLink lg>Large</AsLink>
  </div>
  <div class="d-flex gap-5 as-mt-16 align-items-center">
    <AsLink withIcon sm><i class="as-icon-close"></i><span>Small</span></AsLink>
    <AsLink withIcon><i class="as-icon-close"></i><span>Medium</span></AsLink>
    <AsLink withIcon lg><i class="as-icon-close"></i><span>Large</span></AsLink>
  </div>
  <div class="d-flex gap-5 as-mt-16 align-items-center">
    <AsLink withIcon sm><span>Small</span><i class="as-icon-close"></i></AsLink>
    <AsLink withIcon><span>Medium</span><i class="as-icon-close"></i></AsLink>
    <AsLink withIcon lg><span>Large</span><i class="as-icon-close"></i></AsLink>
  </div>
</template>

<script setup>
import AsLink from "./AsLink.vue";
</script>
