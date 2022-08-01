<template>
  <div class="as-modal__section" :class="className">
    <a class="as-modal__close" @click="closeHandler($event.target)" href="#" title="Close" v-if="close"><i class="as-icon-close"></i></a>
    <slot/>
  </div>
</template>

<script setup>
  import { computed } from 'vue'

  const props = defineProps({
    center: Boolean,
    close: Boolean,
  })

  const className = computed(() => ({
    'as-modal__section--center': props.center,
  }))
  
  const closeHandler = (el) => {
    el.closest('.as-modal').classList.remove('as-modal--visible')
  }
</script>
