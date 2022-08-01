<template>
  <AsButtonFilter withIcon
    ><i class="as-icon-filter"></i><span>Label</span></AsButtonFilter
  >
  <AsButtonFilter withIcon
    ><span>Label</span><i class="as-icon-filter"></i
  ></AsButtonFilter>

  <AsButtonFilter withIcon
    ><i class="as-icon-filter"></i><span>Label</span
    ><i class="as-icon-arrow-down"></i
  ></AsButtonFilter>

  <AsButtonFilter withIcon><i class="as-icon-filter"></i></AsButtonFilter>
</template>

<script setup>
import AsButtonFilter from "./AsButtonFilter.vue";
</script>
