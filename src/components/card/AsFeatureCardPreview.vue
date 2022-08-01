<template>
  <li
    class="as-feature-card as-card as-card__container--xlg as-border-radius-24"
    v-for="item in dataOffer"
    :key="item.id"
  >
    <img :src="item.icon" :alt="item.alt" class="as-width-66 as-mb-24" />
    <h3 class="as-text-20-bold as-lh-26 as-color-primary as-mb-14">
      {{ item.title }}
    </h3>
    <p class="as-text-16 as-lh-24 as-color-secondary-2 as-mb-26">
      {{ item.description }}
    </p>

    <ul class="as-list-icon as-pl-28">
      <li
        class="as-list-icon__item as-list-icon__item--sm as-list-icon__item--sm-blue as-list-icon__item--with-tooltip"
        v-for="list in item.offerList"
        :key="list.id"
      >
        <span>{{ list }}</span>

        <div class="as-tooltip">
          <img
            src="~assets/images/samples/tooltip-icon.svg"
            alt="tooltip icon"
            class="as-width-16"
          />
          <p class="as-tooltip__info as-tooltip__info--top as-text-14 as-lh-24">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa,
            officia praesentium laudantium in fugiat excepturi.
          </p>
        </div>
      </li>
    </ul>
  </li>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import imgEdu from "@/assets/images/samples/organism/vpskvm/offer-education.svg";

const dataOffer = [
  {
    icon: imgEdu,
    alt: "Icon Offer Education",
    title: "E-Learning & Education",
    description:
      "Kelola urusan akademik, dengan penyimpanan data yang lebih besar",
    offerList: [
      "Server Ujian Online",
      "Sistem Akademik",
      "Learning Management",
      "Website Sekolah",
      "Website Universitas",
    ],
  },
];
</script>

<style lang="scss">
@use "@/assets/scss/mixins/breakpoint" as *;

.as-feature-card {
  box-shadow: -80px 80px 80px rgba(35, 44, 79, 0.05);
  list-style-type: none;

  .as-tooltip {
    display: none;
    @include screen(desktop) {
      display: block;
    }
  }
}
</style>
