<template>
  <div class="as-radio">
    <input
      type="radio"
      :id="id"
      :name="name"
      :value="value"
      :required="required"
      @click="$emit('eventClick', $event.target.checked)"
      :checked="checked"
      :disabled="disabled"
    />
    <label :for="id" class="as-radio-label">{{ label }}</label>
  </div>
</template>

<script setup>
const props = defineProps({
  required: Boolean,
  label: String,
  name: {
    type: String,
    default: "radio",
  },
  id: {
    type: String,
    default: "radio",
  },
  value: String,
  checked: Boolean,
  disabled: Boolean,
});
</script>

<style lang="scss">
@use "@/assets/scss/components/radio.scss";
</style>
