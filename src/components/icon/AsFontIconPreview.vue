<template>
  <div v-for="item in items" :key="item.icon" class="col-md-3 as-mb-16">
    <div class="bg-light text-center rounded as-px-8 as-py-16">
      <i :class="'as-icon-' + item.icon"></i>
      <p class="as-text-14 text-muted text-decoration-none text-center as-pt-8">
        {{ titleWords(item.icon) }}
      </p>
    </div>
  </div>
</template>

<script>
import fontIcon from "~/store/data/fontIcon.json";

export default {
  data() {
    return {
      items: fontIcon,
    };
  },
  methods: {
    titleWords(str) {
      let i,
        frags = str.split("-");
      for (i = 0; i < frags.length; i++) {
        frags[i] = frags[i].charAt(0).toUpperCase() + frags[i].slice(1);
      }
      return frags.join(" ");
    },
  },
};
</script>
