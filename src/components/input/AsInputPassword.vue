<template>
  <div class="as-input__password">
    <input
      class="as-input"
      :class="className"
      v-model="password"
      :type="passwordType"
      :placeholder="placeholder"
      :required="required"
      @keyup="$emit('eventKeyup', $event.target.value)"
      @input="$emit('update:modelValue', $event.target.value)"
    />
    <span
      class="as-input__icon"
      :class="passwordIcon"
      @click="switchVisibility"
    ></span>
  </div>
</template>

<script setup>
import { ref } from "vue";

const props = defineProps({
  placeholder: String,
  required: Boolean,
  sm: Boolean,
  disabled: Boolean,
});

const className = computed(() => {
  let baseName = "as-input";

  return {
    [baseName]: true,
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--disable`]: props.disabled,
  };
});

const password = ref("");
const passwordType = ref("password");
const passwordIcon = ref("as-icon-eye-open");

function switchVisibility() {
  passwordType.value = passwordType.value === "password" ? "text" : "password";
  passwordIcon.value =
    passwordIcon.value === "as-icon-eye-open"
      ? "as-icon-eye-close"
      : "as-icon-eye-open";
}
</script>

<style lang="scss" scoped>
@use "@/assets/scss/components/input.scss";
</style>
