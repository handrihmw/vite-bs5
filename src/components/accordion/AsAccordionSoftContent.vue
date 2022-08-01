<template>
  <div class="as-accordion-soft__body" v-if="visible()">
    <div class="as-accordion-soft__content">
      <slot />
    </div>
  </div>
</template>

<script setup>
import { inject } from "vue";

const visible = inject("visible");
</script>
