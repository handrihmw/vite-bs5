<template>
  <div class="">
    <div class="as-input__group-dropdown" @click="show" :class="className">
      <span class="as-input__group-input">{{ text }}</span>
    </div>
    <transition name="slide">
      <div
        class="as-input__group-dropdown-menu as-px-16 as-py-16"
        v-if="showDropdown"
      >
        <ul>
          <slot />
        </ul>
      </div>
    </transition>
  </div>
</template>

<script setup>
const showDropdown = ref(false);
const show = () => {
  showDropdown.value = !showDropdown.value;
};

const props = defineProps({
  text: {
    default: "Dropdown",
    type: String,
  },
  disabled: Boolean,
});

const className = computed(() => {
  let baseName = "as-input__group-dropdown";

  return {
    [baseName]: true,
    [`${baseName}--disable`]: props.disabled,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/input.scss";
</style>
