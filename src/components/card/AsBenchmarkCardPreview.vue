<template>
  <li
    class="as-benchmark-card as-card as-card__container--benchmark as-card__section justify-content-between as-border-radius-12 as-mb-0"
    v-for="item in dataPerformance"
    :key="item.id"
  >
    <h3 class="as-text-16-semibold as-lh-24 as-color-green">
      {{ item.title }}
    </h3>
    <div>
      <p class="as-text-56 as-lh-64">
        {{ item.value
        }}<span class="as-text-24-bold as-lh-32 as-ml-4">{{ item.unit }}</span>
      </p>
      <p class="as-text-16 as-lh-24 as-color-secondary-2">Up to</p>
    </div>
  </li>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";

const dataPerformance = [
  {
    title: "Bandwidth Speed",
    value: "30",
    unit: "Mbps",
  },
];
</script>

<style lang="scss">
@use "@/assets/scss/mixins/breakpoint" as *;

.as-benchmark-card {
  min-width: 15.9375rem;
}
</style>
