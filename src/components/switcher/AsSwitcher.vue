<template>
  <div class="as-switch">
    <input
      @click="$emit('check', $event.target.checked)"
      :id="id"
      :name="name"
      role="switch"
      type="checkbox"
      :value="value"
      :checked="checked"
      :disabled="disabled"
    />
    <label :for="id"></label>
  </div>
</template>

<script setup>
const props = defineProps({
  id: {
    type: String,
    required: true,
  },
  name: String,
  value: String,
  checked: Boolean,
  disabled: Boolean,
});
</script>

<style lang="scss">
@use "@/assets/scss/components/switch";
</style>
