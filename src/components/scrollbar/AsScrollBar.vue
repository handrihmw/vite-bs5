<template>
  <div class="as-scrollbar" :class="className">
    <slot />
  </div>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  scrollX: Boolean,
  scrollY: Boolean,
});

const className = computed(() => ({
  "as-scrollbar__horizontal": props.scrollX,
  "as-scrollbar__vertical": props.scrollY,
}));
</script>
