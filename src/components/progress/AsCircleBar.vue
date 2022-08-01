<template>
  <div
    class="as-circlebar"
    :style="{ width: size + 'px', height: size + 'px', color: changeColor }"
    :data-pct="progressNumber"
  >
    <svg
      :width="size"
      :height="size"
      :viewPort="'0 0 ' + size + ' ' + size"
      version="1.1"
      xmlns="http://www.w3.org/2000/svg"
    >
      <circle
        class="ring"
        :stroke="ringColor"
        :r="ring"
        :cx="size / 2"
        :cy="size / 2"
        :stroke-width="width"
        fill="none"
      ></circle>
      <circle
        class="as-circlebar__circle"
        :style="{ stroke: changeColor }"
        :stroke="progressColor"
        :r="ring"
        :cx="size / 2"
        :cy="size / 2"
        :stroke-width="width"
        fill="none"
        :stroke-dasharray="dashArray"
        :stroke-dashoffset="dashOffset"
      ></circle>
    </svg>
  </div>
</template>

<script setup>
import { computed } from "vue";

const percentage = computed(() => {
  return (props.valueNow / props.valueMax) * 100;
});

const ring = computed(() => {
  return props.size / 2 - props.width / 2;
});

const progressNumber = computed(() => {
  return props.showNumber && parseInt(percentage.value);
});

const dashArray = computed(() => {
  return 2 * Math.PI * ring.value;
});

const dashOffset = computed(() => {
  return dashArray.value * (1 - percentage.value / 100);
});

const changeColor = computed(() => {
  let color = "var(--as-color-gray)";
  if (progressNumber.value > 0 && progressNumber.value <= 59) {
    color = "var(--as-color-red)";
  } else if (progressNumber.value >= 60 && progressNumber.value <= 89) {
    color = "var(--as-color-orange)";
  } else if (progressNumber.value >= 90) {
    color = "var(--as-color-green)";
  }
  return color;
});

const props = defineProps({
  valueNow: {
    type: String,
    default: "10",
  },
  valueMax: {
    type: String,
    default: "100",
  },
  size: {
    type: String,
    default: "100",
  },
  width: {
    type: String,
    default: "8",
  },
  ringColor: {
    type: String,
    default: "var(--as-color-gray)",
  },
  progressColor: {
    type: String,
    default: null,
  },
  textColor: {
    type: String,
    default: "var(--as-color-gray)",
  },
  showNumber: {
    type: Boolean,
    default: true,
  },
});
</script>

<style lang="scss">
@use "@/assets/scss/components/circlebar.scss";
</style>
