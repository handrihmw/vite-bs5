<template>
  <section class="as-section-blue as-py-32 as-px-20">
    <div class="as-section__container">
      <div class="as-section__flex as-gap-120">
        <div class="as-section__image as-mb-32 as-mx-20">
          <img
            src="~assets/images/samples/organism/cloudvpshosting/illust-os-2.svg"
            alt="Illustration OS"
            loading="lazy"
          />
        </div>

        <div>
          <h2 class="as-section__title as-mb-32">
            Ganti OS Dengan Mudah di Cloud VPS Niagahoster
          </h2>
          <p class="as-section__description as-mb-32">
            Nikmati beragam OS dengan teknologi dan fitur terbaik dari VPS murah
            terbaik di Indonesia. Kelola website dan segala kebutuhan online
            Anda tanpa repot di Niagahoster!
          </p>
          <button class="as-btn as-btn--primary as-btn--fluid">
            Pesan Sekarang
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss">
@use "@/assets/scss/components/section.scss";
@use "@/assets/scss/mixins/breakpoint" as *;

.as-section-blue {
  @include screen(desktop) {
    padding: 2.1875rem 1.25rem;
  }

  .as-section__image {
    @include screen(desktop) {
      min-width: 15.625rem;
      margin-bottom: unset;
      margin-inline: unset;
    }
  }

  .as-section__title {
    font-size: 2rem;
    line-height: 2.625rem;
  }

  .as-btn {
    @include screen(desktop) {
      width: fit-content;
      padding-inline: 4.875rem;
    }
  }
}
</style>
