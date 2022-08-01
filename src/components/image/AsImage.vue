<template>
  <img
    class="as-image lazyload blur-up"
    :class="className"
    loading="lazy"
    alt="image"
  />
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  bottomRounded: Boolean,
  fill: Boolean,
  fluid: Boolean,
  fluidHeight: Boolean,
  fluidWidth: Boolean,
  leftRounded: Boolean,
  rightRounded: Boolean,
  rounded: Boolean,
  topRounded: Boolean,
});

const className = computed(() => ({
  "as-image--bottom-rounded": props.bottomRounded,
  "as-image--fill": props.fill,
  "as-image--fluid": props.fluid,
  "as-image--fluid-height": props.fluidHeight,
  "as-image--fluid-width": props.fluidWidth,
  "as-image--left-rounded": props.leftRounded,
  "as-image--right-rounded": props.rightRounded,
  "as-image--rounded": props.rounded,
  "as-image--top-rounded": props.topRounded,
}));
</script>

<style lang="scss">
@use "@/assets/scss/mixins/border" as *;

.as-image {
  image-rendering: auto;

  &--bottom-rounded {
    @include border-radius(0, 0, 16px, 16px);
  }

  &--left-rounded {
    @include border-radius(16px, 0, 0, 16px);
  }

  &--right-rounded {
    @include border-radius(0, 16px, 16px, 0);
  }

  &--rounded {
    @include border-radius(16px, 16px, 16px, 16px);
  }

  &--top-rounded {
    @include border-radius(16px, 16px, 0, 0);
  }

  &--fill {
    object-fit: fill;
  }

  &--fluid {
    height: 100%;
    width: 100%;

    &-height {
      height: 100%;
    }

    &-width {
      width: 100%;
    }
  }
}
</style>
