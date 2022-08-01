<template>
  <div class="as-input as-input__select" :class="className">
    <select
      name="as-input__select"
      :value="modelValue"
      v-bind="filteredAttrs"
      @change="changeHandler($event.target.value)"
    >
      <option
        v-for="(item, index) in options"
        :key="index"
        :selected="selected == item.value"
        :value="item.value"
      >
        {{ item.option }}
      </option>
    </select>
  </div>
</template>

<script>
export default {
  inheritAttrs: false,
};
</script>

<script setup>
import { computed, useAttrs } from "vue";

const props = defineProps({
  required: Boolean,
  options: {
    type: Array,
    default: [
      {
        value: "",
        option: "Select",
      },
      {
        value: "1",
        option: "Select One",
      },
      {
        value: "2",
        option: "Select Two",
      },
      {
        value: "3",
        option: "Select Three",
      },
      {
        value: "4",
        option: "Select Four",
      },
    ],
  },
  selected: String,
  sm: Boolean,
  modelValue: [Number, String],
});

const attrs = useAttrs();

const filteredAttrs = computed(() => {
  let result = {};
  for (let key in attrs) {
    if (key != "class") {
      Object.assign(result, { [`${key}`]: attrs[key] });
    }
  }
  return result;
});

const emit = defineEmits(["update:modelValue", "eventChange"]);

const changeHandler = (value) => {
  emit("update:modelValue", value);
  emit("eventChange", value);
};

const className = computed(() => {
  const result = {
    "as-input__select--sm": props.sm,
  };

  if (typeof attrs.class != "undefined") {
    Object.assign(result, { [`${useAttrs().class}`]: true });
  }

  return result;
});
</script>

<style lang="scss">
@use "@/assets/scss/components/input.scss";
</style>
