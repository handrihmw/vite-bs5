<template>
  <div class="as-product-recommendation-card">
    <AsCard border borderSoft>
      <AsCardContainer class="d-flex flex-column gap-4 justify-content-between">
        <div>
          <img
            src="~assets/images/product-icon/icon-wordpress-hosting.svg"
            class="as-width-54 as-height-54 as-mb-24"
            loading="lazy"
            alt="icon wordpress hosting"
          />
          <h3 class="as-text-20-bold as-mb-8 as-lh-26">Wordpress Hosting</h3>
          <p class="as-text-14 as-color-secondary as-lh-24">
            Hosting dengan performa paling optimal untuk mengelola website
            WordPress Anda
          </p>
        </div>

        <div>
          <p class="as-text-12 as-color-secondary-2 as-mt-4 as-lh-24">
            Mulai dari
          </p>
          <h3 class="as-text-24-bold as-color-orange as-mb-24 as-lh-32">
            Rp 26.813
            <span class="as-text-20-bold as-color-primary as-lh-26"
              >/bulan</span
            >
          </h3>

          <AsButton anchor href="#" primary fluid class="as-mt-4">
            Lihat Detail
          </AsButton>
        </div>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardSection from "./AsCardSection.vue";
import AsButton from "../button/AsButton.vue";
</script>

<style lang="scss">
@use "@/assets/scss/mixins/breakpoint" as *;
.as-product-recommendation-card {
  max-width: 15.9375rem;
  min-width: 15.9375rem;
  border-radius: 1rem;
  flex-direction: column;
  justify-content: space-between;
  gap: 1.75rem;

  @include screen(desktop) {
    max-width: 21.875rem;
    min-width: 21.875rem;
  }
}
</style>
