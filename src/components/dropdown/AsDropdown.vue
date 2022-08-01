<template>
  <div
    class="as-dropdown"
    :class="className"
    :data-value="text"
    :data-list="listItem"
  >
    <div class="as-dropdown__menu" @click="toggleDropdown()">
      <div class="text as-text-16">
        <span>{{ text }}</span>
      </div>
      <div class="label as-text-16 as-color-disable" v-if="withLabel">
        <span>{{ label }}</span>
      </div>
      <div class="icon" :class="{ extended: visible }">
        <i class="as-icon-arrow-down"></i>
      </div>
      <ul :class="{ hidden: !visible, visible }">
        <li
          :class="{ current: item === text }"
          v-for="item in listItem"
          :key="item.id"
          @click="select(item)"
          class="as-text-16-semibold as-color-secondary"
        >
          {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
import { computed } from "vue";
const text = ref("Pilih salah satu");

const visible = ref(false);
const toggleDropdown = () => {
  visible.value = !visible.value;
};

const select = (option) => {
  text.value = option;
};

const props = defineProps({
  sm: Boolean,
  disabled: Boolean,
  left: Boolean,
  right: Boolean,
  withLabel: Boolean,
  label: {
    default: "Dropdown label",
    type: String,
  },
  listItem: {
    type: Array,
    default: ["label 1", "label 2", "label 3", "label 4"],
  },
});

const className = computed(() => {
  let baseName = "as-dropdown";

  return {
    [`${baseName}--sm`]: props.sm,
    [`${baseName}--left`]: props.left,
    [`${baseName}--right`]: props.right,
    [`${baseName}--disable`]: props.disabled,
  };
});
</script>

<style lang="scss">
@use "@/assets/scss/components/dropdown.scss";
</style>
