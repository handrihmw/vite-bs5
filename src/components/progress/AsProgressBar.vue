<template>
  <div
    class="as-progress-bar"
    role="progressbar"
    :aria-valuenow="valuenow"
    :aria-valuemin="valuemin"
    :aria-valuemax="valuemax"
    :style="{ width: percentage }"
  ></div>
</template>

<script setup>
import { computed } from "vue";

const percentage = computed(() => {
  return (props.valuenow / props.valuemax) * 100 + "%";
});

const props = defineProps({
  valuenow: String,
  valuemin: {
    type: String,
    default: 0,
  },
  valuemax: {
    type: String,
    default: 100,
  },
});
</script>
