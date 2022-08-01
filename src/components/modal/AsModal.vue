<template>
  <div class="as-modal">
    <div class="as-modal__dialog">
      <div class="as-modal__container" :class="className">
        <slot/>
      </div>
    </div>
  </div>
</template>

<script setup>
  import { computed } from 'vue'
  
  const props = defineProps({
    xs: Boolean,
    sm: Boolean,
    md: Boolean,
    lg: Boolean,
  })

  const className = computed(() => ({
    'as-modal__container--xs': props.xs,
    'as-modal__container--sm': props.sm,
    'as-modal__container--md': props.md,
    'as-modal__container--lg': props.lg,
  }))
</script>

<style lang="scss">
  @use '@/assets/scss/components/modal';
</style>
