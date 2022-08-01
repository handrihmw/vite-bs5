<template>
  <textarea
    :class="className"
    :disabled="disabled"
    :value="modelValue"
    @input="$emit('update:modelValue', $event.target.value)"
  >
  </textarea>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  disabled: Boolean,
  modelValue: String,
});

const className = computed(() => {
  let baseName = "as-textarea";
  return {
    [baseName]: true,
    [`${baseName}--disable`]: props.disabled,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/textarea.scss";
</style>
