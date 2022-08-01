<template>
  <ul>
    <li v-for="item in items" :key="item.id" class="as-mb-48">
      <h5 class="as-mb-16">{{ item.name }}</h5>
      <ul class="row">
        <li v-for="col in item.colors" :key="col.id" class="col-md-3 as-mb-16">
          <div class="color__wrapper">
            <div :class="col.class" class="color__box as-mb-16"></div>
            <p class="as-text-16-bold">{{ col.name }}</p>
            <p class="as-text-16 as-mt-8">{{ col.hex }}</p>
            <p class="as-color-secondary as-mt-8 as-mb-8">
              Use <code>.{{ col.var }}</code> classes
            </p>
            <ul class="d-flex flex-row flex-wrap gap-3">
              <li v-for="grad in col.hexGrad" :key="grad.id">
                <p>{{ grad }}</p>
              </li>
            </ul>
          </div>
        </li>
      </ul>
    </li>
  </ul>
</template>

<script setup>
import colorsData from "~/store/data/colors.json";
const items = colorsData;
</script>

<style lang="scss" scoped>
@use "@/assets/scss/mixins/breakpoint" as *;
ul {
  margin: 0;
  padding: 0;
  gap: 1.5rem;
  li {
    list-style-type: none;
    padding: 0;
    .color__box {
      height: 120px;
      width: 100%;
      border-radius: 6px;
    }
  }
}
</style>
