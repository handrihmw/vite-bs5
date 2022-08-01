<template>
  <li
    v-if="active"
    aria-current="page"
    class="as-breadcrumb__item"
    :class="className"
  >
    <slot />
  </li>
  <li v-else class="as-breadcrumb__item" :class="className">
    <a :href="path" v-if="anchor"><slot /></a>
    <router-link :to="path" v-else><slot /></router-link>
  </li>
</template>

<script setup>
import { computed } from "vue";

const props = defineProps({
  active: {
    default: false,
    type: Boolean,
  },
  anchor: Boolean,
  path: {
    default: "/",
    type: String,
  },
});

const className = computed(() => ({
  "as-breadcrumb__item--active": props.active,
}));
</script>
