<template>
  <div class="as-checkbox">
    <div class="as-checkbox__item">
      <label class="as-text-16-semi-bold as-color-secondary-2"
        >{{ label }}
        <input
          type="checkbox"
          :required="required"
          :value="value"
          @click="$emit('eventClick', $event.target.checked)"
          :checked="checked"
        />
        <slot />
        <span class="checkmark"></span>
      </label>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  required: Boolean,
  label: String,
  value: null,
  checked: Boolean,
});
</script>

<style lang="scss">
@use "@/assets/scss/components/checkbox.scss";
</style>
