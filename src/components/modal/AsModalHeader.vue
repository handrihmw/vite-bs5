<template>
  <div class="as-modal__header">
    <a class="as-modal__close" @click="closeHandler($event.target)" href="#" title="Close" v-if="close"><i class="as-icon-close"></i></a>
    <slot/>
  </div>
</template>

<script setup>
  const props = defineProps({
    close: Boolean,
  })
  
  const closeHandler = (el) => {
    el.closest('.as-modal').classList.remove('as-modal--visible')
  }
</script>

