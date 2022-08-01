<template>
  <div class="row">
    <div class="as-theme-choice-card">
      <AsCard border>
        <AsCardContainer md>
          <h2 class="as-text-18-bold as-color-primary as-mb-24">
            Cepatlakoo 25 Website
          </h2>
          <AsCardSection class="as-mb-4">
            <AsCardImage
              installed
              class="as-border-radius-8 as-mb-24"
              loading="lazy"
            />

            <p class="as-text-14 as-color-secondary-2 as-mb-8">
              Cepatlakoo adalah theme WordPress khusus untuk toko online yang
              sangat mudah untuk digunakan dan sudah dilengkapi dengan sistem
              checkout yang sederhana...
            </p>

            <AsLink withIcon sm>
              <span>Lihat fitur lengkapnya</span>
              <i class="as-icon-arrow-right"></i
            ></AsLink>
          </AsCardSection>
        </AsCardContainer>
        <AsCardSection top>
          <AsCardContainer md>
            <AsCardSection flex class="justify-content-between as-mb-24">
              <p class="as-text-14 as-color-secondary-2">Harga</p>
              <p class="as-text-16-bold as-color-orange">Rp 499.999</p>
            </AsCardSection>
            <AsButton primary fluid>Beli Sekarang</AsButton>
          </AsCardContainer>
        </AsCardSection>
      </AsCard>
    </div>

    <div class="as-theme-choice-card">
      <AsCard border disabled>
        <AsCardContainer md>
          <h2 class="as-text-18-bold as-color-primary as-mb-24">
            Cepatlakoo 25 Website
          </h2>
          <AsCardSection class="as-mb-4">
            <AsCardImage
              installed
              class="as-border-radius-8 as-mb-24"
              loading="lazy"
            />

            <p class="as-text-14 as-color-secondary-2 as-mb-8">
              Cepatlakoo adalah theme WordPress khusus untuk toko online yang
              sangat mudah untuk digunakan dan sudah dilengkapi dengan sistem
              checkout yang sederhana...
            </p>

            <AsLink withIcon sm>
              <span>Lihat fitur lengkapnya</span>
              <i class="as-icon-arrow-right"></i
            ></AsLink>
          </AsCardSection>
        </AsCardContainer>
        <AsCardSection top>
          <AsCardContainer md>
            <AsCardSection flex class="justify-content-between as-mb-24">
              <p class="as-text-14 as-color-secondary-2">Harga</p>
              <p class="as-text-16-bold as-color-orange">Rp 499.999</p>
            </AsCardSection>
            <AsButton primary fluid>Beli Sekarang</AsButton>
          </AsCardContainer>
        </AsCardSection>
      </AsCard>
    </div>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardImage from "./AsCardImage.vue";
import AsCardSection from "./AsCardSection.vue";

import AsButton from "../button/AsButton.vue";
import AsLink from "../button/AsLink.vue";
</script>

<style lang="scss" scoped>
.as-theme-choice-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 21rem;
    height: auto;
  }
}
</style>
