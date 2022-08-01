<template>
  <div class="as-belt overflow-hidden">
    <div class="as-belt__wrapper as-gap-32">
      <div class="as-belt__image">
        <img
          src="~assets/images/banner/campaign-belt-cloud-hosting-illustration-mobile.svg"
          alt="campaign cloud hosting illustration"
          loading="lazy"
          class="d-block d-lg-none"
          width="100%"
          height="100%"
        />
        <img
          src="~assets/images/banner/campaign-belt-cloud-hosting-illustration-desktop.svg"
          alt="campaign cloud hosting illustration"
          loading="lazy"
          class="d-none d-lg-block"
          width="100%"
          height="100%"
        />
      </div>
      <div class="as-belt-content">
        <h2 class="as-belt-content__title">Beli Hosting Gratis 2 Domain!</h2>
        <p class="as-belt-content__description">
          Beli layanan <span class="as-text-bold">Cloud Hosting</span> gratis
          domain <span class="as-text-bold">.com</span> dan
          <span class="as-text-bold">.site</span>. Klaim sekarang sebelum promo
          berakhir!
        </p>
      </div>
      <div class="as-belt__button d-block d-lg-none">
        <a href="#" class="as-btn as-btn--primary as-btn--fluid"
          >Dapatkan Promo</a
        >
      </div>
      <div class="as-belt__button d-none d-lg-block">
        <a href="#" class="as-btn as-btn--primary as-btn--fluid"
          >Lihat Semua Promo</a
        >
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss">
@use "@/assets/scss/components/belt";
</style>
