<template>
  <li :aria-setsize="size" :aria-posinset="posInSet" class="as-nav-line__item">
    <a 
      :aria-selected="posInSet == activeTab"
      class="as-nav-line__link as-btn-icon" 
      :class="{'is-active': posInSet == activeTab}"
      @click="clickHandler"
    >
      <slot/>
    </a>
  </li>
</template>

<script setup>
  import { inject } from 'vue'
  
  const props = defineProps({
    active: Boolean,
    posInSet: {
      required: true,
      type: Number,
    },
  })
  
  const size = inject('size', 1)
  
  const activeTab = inject('activeTab')
  
  if (props.active) {
    activeTab.value = props.posInSet
  }
  
  const clickHandler = () => {
    activeTab.value = props.posInSet
  }
</script>
