<template>
  <div
    class="as-card-color as-card-testimony-v2 text-center d-flex flex-column flex-lg-row"
  >
    <div>
      <h3 class="as-card-testimony-v2__rating">4,8</h3>
      <div
        class="as-rating as-rating--lg as-rating--four-half as-rating--center as-mb-20"
      >
        <em class="as-icon-star-outline" />
        <em class="as-icon-star-outline" />
        <em class="as-icon-star-outline" />
        <em class="as-icon-star-outline" />
        <em class="as-icon-star-outline" />
      </div>
      <a href="#" class="as-card-testimony-v2__reviews">2,525 reviews</a>
      <a href="#" class="as-btn as-btn--primary as-btn--fluid">
        Buktikan Sendiri
      </a>
    </div>

    <ul class="text-start row">
      <li
        class="col-lg-4 mb-4 mb-lg-0"
        v-for="item in dataRating"
        :key="item.id"
      >
        <h4 class="as-card-testimony-v2__title">
          {{ item.title }}
        </h4>
        <div class="as-rating as-rating--md as-rating--five as-mb-24">
          <em class="as-icon-star-outline" />
          <em class="as-icon-star-outline" />
          <em class="as-icon-star-outline" />
          <em class="as-icon-star-outline" />
          <em class="as-icon-star-outline" />
        </div>
        <p class="as-card-testimony-v2__description">
          {{ item.description }}
        </p>
      </li>
    </ul>
  </div>
</template>

<script setup>
const dataRating = [
  {
    title: "“Niagahoster hosting terbaik!”",
    description:
      "“Selama saya menggunakan hosting, Niagahoster merupakan yang terbaik dari semuanya, pelayanan cepat, harga terjangkau, dan juga sangat bisa diandalkan, membuat website wordpress juga sangat mudah sekali di Niagahoster.”",
  },
  {
    title: "“Best Hosting in Town!”",
    description:
      "“Personally, I satisfied with all services in Niagahoster, easy to check billing, make payment, and also reminder notification. Customer Service is always support whenever I need help. Thank you.”",
  },
  {
    title: "“Ramah Untuk Newbie”",
    description:
      "“Aku newbie banget di dunia website, jadi suka bingung kalau ini gimana kalau itu gimana. Untungnya ada banyak tutorial yang niagahoster kasih tinggal dicari aja biasanya ketemu. Kalau tutorialnya ga berhasil bisa langsung hubungin cs aja dan diarahin dengan sabar bangeeeeeet. Dan works! apa yang aku mau bisa diarahin sama cs nya. Good jooob~~~”",
  },
];
</script>

<style lang="scss">
@use "@/assets/scss/components/card-testimony.scss";
</style>
