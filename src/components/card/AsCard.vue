<template>
  <div :class="className">
    <slot />
  </div>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  label: Boolean,
  play: Boolean,
  white: Boolean,
  blue: Boolean,
  gray: Boolean,
  soft: Boolean,
  border: Boolean,
  borderSoft: Boolean,
  icon: Boolean,
  dashed: Boolean,
  center: Boolean,
  disabled: Boolean,
  gradientBlue: Boolean,
  yellow: Boolean,
  noShadow: Boolean,
});

const className = computed(() => {
  let baseName = "as-card";

  return {
    [baseName]: true,
    [`${baseName}--label`]: props.label,
    [`${baseName}--play`]: props.play,
    [`${baseName}--white`]: props.white,
    [`${baseName}--blue`]: props.blue,
    [`${baseName}--gray`]: props.gray,
    [`${baseName}--soft`]: props.soft,
    [`${baseName}--border`]: props.border,
    [`${baseName}--icon`]: props.icon,
    [`${baseName}--yellow`]: props.yellow,
    [`${baseName}--dashed`]: props.dashed,
    [`${baseName}--center`]: props.center,
    [`${baseName}--disabled`]: props.disabled,
    [`${baseName}--border-soft`]: props.borderSoft,
    [`${baseName}--gradient-blue`]: props.gradientBlue,
    [`${baseName}--no-shadow`]: props.noShadow,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/card.scss";
</style>
