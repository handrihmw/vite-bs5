<template>
  <input
    type="text"
    v-bind="$attrs"
    :class="className"
    :disabled="disabled"
    :value="modelValue ?? value"
    @input="$emit('update:modelValue', $event.target.value)"
    @keyup="$emit('eventKeyup', $event.target.value)"
    @keyup.enter="$emit('eventEnter')"
  />

  <span class="as-input__icon" v-if="withIcon">
    <slot />
  </span>
</template>

<script>
export default {
  inheritAttrs: false,
};
</script>

<script setup>
import { ref, computed } from "vue";

const props = defineProps({
  disabled: Boolean,
  search: Boolean,
  groupInput: Boolean,
  groupLeft: Boolean,
  groupRight: Boolean,
  groupPrefix: String,
  withIcon: Boolean,
  noLeft: Boolean,
  noRight: Boolean,
  modelValue: [Number, String],
  value: [Number, String],
});

const className = computed(() => {
  let baseName = "as-input";

  return {
    [baseName]: true,
    [`${baseName}__search`]: props.search,
    [`${baseName}__group-input`]: props.groupInput,
    [`${baseName}__group-input--left`]: props.groupLeft,
    [`${baseName}__group-input--right`]: props.groupRight,
    [`${baseName}--disable`]: props.disabled,
    [`as-border-radius-no-left`]: props.noLeft,
    [`as-border-radius-no-right`]: props.noRight,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/input.scss";
</style>
