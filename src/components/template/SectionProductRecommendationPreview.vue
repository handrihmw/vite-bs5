<template>
  <section class="as-section-white as-pt-32">
    <h2 class="as-section__title">
      Rekomendasi Produk Hosting Lainnya dari Niagahoster
    </h2>

    <ul class="as-slider-simple as-mt-32 as-py-32 as-mx-auto as-max-width-1110">
      <li
        class="as-product-recommendation-card as-card as-card--border as-card--border__soft as-card__container d-flex flex-column gap-4 justify-content-between"
        v-for="item in dataProductCard"
        :key="item.id"
      >
        <div>
          <img
            :src="item.src"
            class="as-width-54 as-height-54 as-mb-24"
            loading="lazy"
            alt="icon wordpress hosting"
          />
          <h3 class="as-text-20-bold as-mb-8 as-lh-26">{{ item.title }}</h3>
          <p class="as-text-14 as-color-secondary as-lh-24">
            {{ item.description }}
          </p>
        </div>
        <div>
          <p class="as-text-14 as-color-secondary-2 as-lh-24">Mulai dari</p>
          <h3 class="as-text-24-bold as-color-orange mb-4 as-lh-32">
            {{ item.price }}
            <span class="as-text-20-bold as-color-primary as-lh-26"
              >/bulan</span
            >
          </h3>

          <a
            :href="item.href"
            target="_blank"
            class="as-btn as-btn--primary as-btn--fluid"
          >
            Lihat Detail
          </a>
        </div>
      </li>
    </ul>
  </section>
</template>

<script setup>
import imgWPH from "@/assets/images/product-icon/icon-wordpress-hosting.svg";
import imgCH from "@/assets/images/product-icon/icon-cloud-hosting.svg";
import imgEH from "@/assets/images/product-icon/icon-email-hosting.svg";

const dataProductCard = [
  {
    src: imgWPH,
    title: "Wordpress Hosting",
    description:
      "Hosting dengan performa paling optimal untuk mengelola website WordPress Anda",
    price: "Rp 26.813",
    href: "https://www.niagahoster.co.id/wordpress-hosting",
  },
  {
    src: imgCH,
    title: "Cloud Hosting",
    description:
      "Layanan hosting dengan resource terbesar untuk kebutuhan website skala besar Anda",
    price: "Rp 137.500",
    href: "https://www.niagahoster.co.id/cloud-hosting",
  },
  {
    src: imgEH,
    title: "Email Hosting",
    description:
      "Kirim email sepuasnya dengan limit yang besar, dilengkapi dengan keamanan yang termutakhir.",
    price: "Rp 80.000",
    href: "https://www.niagahoster.co.id/email-hosting",
  },
];
</script>

<style lang="scss" scoped>
@use "@/assets/scss/mixins/breakpoint" as *;

.as-section-white {
  @include screen(desktop) {
    padding-block: 5.5rem;
  }

  .as-section__title {
    @include screen(desktop) {
      text-align: center;
      margin-bottom: 3.5rem;
    }
  }
}
</style>
