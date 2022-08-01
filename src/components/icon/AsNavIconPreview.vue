<template>
  <ul class="row as-gap-48">
    <li class="col-md-2 text-center" v-for="item in navIcon" :key="item.id">
      <img
        :src="item.src"
        :alt="item.alt"
        width="40"
        height="40"
        loading="lazy"
      />
      <p class="as-text-14 as-color-secondary as-pt-8">
        {{ item.name }}
      </p>
    </li>
  </ul>
</template>

<script setup>
import navIcon from "~/store/data/navIcon.json";
</script>

<style></style>
