<template>
  <AsButtonOutline
    v-if="outline"
    :anchor="anchor"
    :soft="soft"
    :danger="danger"
    :dark="dark"
    :primary="primary"
    :secondary="secondary"
    :shade="shade"
    :success="success"
    :disabled="disabled"
    :class="className"
  >
    <slot />
  </AsButtonOutline>
  <AsButton
    v-else
    :anchor="anchor"
    :soft="soft"
    :danger="danger"
    :dark="dark"
    :primary="primary"
    :secondary="secondary"
    :shade="shade"
    :success="success"
    :disabled="disabled"
    :class="className"
  >
    <slot />
  </AsButton>
</template>

<script setup>
import { computed } from "vue";
import AsButton from "./AsButton.vue";
import AsButtonOutline from "./AsButtonOutline.vue";

const props = defineProps({
  anchor: Boolean,
  outline: Boolean,
  soft: Boolean,
  danger: Boolean,
  dark: Boolean,
  primary: Boolean,
  secondary: Boolean,
  shade: Boolean,
  success: Boolean,
  disabled: Boolean,
});

const className = computed(() => {
  let baseName = "as-btn-icon";

  return {
    [baseName]: true,
    [`${baseName}--soft`]: props.soft && !props.disabled,
    [`${baseName}--danger`]: props.danger && !props.disabled,
    [`${baseName}--dark`]: props.dark && !props.disabled,
    [`${baseName}--primary`]: props.primary && !props.disabled,
    [`${baseName}--secondary`]: props.secondary && !props.disabled,
    [`${baseName}--shade`]: props.shade && !props.disabled,
    [`${baseName}--success`]: props.success && !props.disabled,
    [`${baseName}--disabled`]: props.disabled,
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--md`]: props.md,
    "as-btn-icon--sm": true,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/button.scss";
@use "@/assets/scss/components/button-icon.scss";
</style>
