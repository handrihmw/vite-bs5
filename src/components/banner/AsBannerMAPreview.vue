<template>
  <div class="as-banner-solid">
    <div class="as-banner-solid__image">
      <img
        src="~assets/images/banner/campaign-belt-cloud-hosting-illustration-desktop.svg"
        alt="campaign cloud hosting illustration"
        loading="lazy"
        width="100%"
        height="100%"
        class="d-none d-lg-block"
      />
      <img
        src="~assets/images/banner/campaign-belt-cloud-hosting-illustration-mobile.svg"
        alt="campaign cloud hosting illustration"
        loading="lazy"
        width="100%"
        height="100%"
        class="d-block d-lg-none"
      />
    </div>
    <div class="d-lg-flex justify-content-lg-between w-100">
      <div class="as-banner-solid__content">
        <h2 class="as-banner-solid__title">Gratis 2 Domain!</h2>
        <em class="d-none d-lg-block">|</em>
        <p class="as-banner-solid__description">
          Beli layanan Cloud Hosting sekarang dan dapatkan domain
          <span class="as-text-bold">.com</span> dan
          <span class="as-text-bold">.site</span> gratis!
        </p>
      </div>

      <div class="as-banner-solid__button">
        <a href="#" class="as-btn as-btn--sm as-btn--fluid as-btn--primary"
          >Beli Sekarang</a
        >
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss">
@use "@/assets/scss/components/banner-solid";
</style>
