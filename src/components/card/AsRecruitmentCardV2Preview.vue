<template>
  <li
    class="as-recruitment-card-v2 as-card__container--xxlg"
    v-for="item in dataRecruitmentV2"
    :key="item.id"
  >
    <img
      :src="item.src"
      alt="recruitment process 1"
      class="as-recruitment-card-v2__image"
      loading="lazy"
    />
    <h3 class="as-text-20-bold as-color-primary as-lh-26 as-mb-18">
      {{ item.title }}
    </h3>
    <p class="as-text-16 as-color-secondary as-lh-24">
      {{ item.description }}
    </p>
  </li>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import imgRec1 from "@/assets/images/samples/organism/lpkarir/recruitment-1.svg";

const dataRecruitmentV2 = [
  {
    src: imgRec1,
    title: "Online Application",
    description:
      "Apply through our Career Page or external job portals that’s officially posted by Niagahoster.",
  },
];
</script>

<style lang="scss">
@use "@/assets/scss/mixins/breakpoint" as *;

.as-recruitment-card-v2 {
  position: relative;
  min-height: 12.8125rem;
  list-style-type: none;

  &__image {
    position: absolute;
    top: 0.375rem;
    left: 1rem;
    opacity: 0.2;
  }
}
</style>
