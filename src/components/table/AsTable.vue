<template>
  <table class="table as-table" :class="className">
    <slot />
  </table>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  striped: Boolean,
});

const className = computed(() => ({
  "as-table__striped": props.striped,
}));
</script>

<style lang="scss">
@use "../../assets/scss/components/table";
</style>
