<template>
  <ul class="as-nav-line__tabs">
    <slot />
  </ul>
</template>

<script setup>
import { provide, ref, watch } from "vue";

const props = defineProps({
  tabSize: {
    required: true,
    type: Number,
  },
});

const size = ref(props.tabSize);

provide("size", size);

const activeTab = ref(1);

provide("activeTab", activeTab);

const emit = defineEmits(["activeTabChange"]);

watch(activeTab, (newPos) => {
  emit("activeTabChange", newPos);
});
</script>

<style lang="scss">
@use "@/assets/scss/components/tab-line";
</style>
