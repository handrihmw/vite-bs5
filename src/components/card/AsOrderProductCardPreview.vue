<template>
  <div class="as-order-product-card">
    <AsCard border noShadow>
      <AsCardContainer md>
        <AsCardSection flex class="gap-3 as-mb-24">
          <img
            src="~assets/images/product-icon/email-hosting.svg"
            class="as-width-54 as-height-54"
            loading="lazy"
            alt="image"
          />
          <div>
            <h2 class="as-text-16-bold as-mb-8">Unlimited Hosting</h2>
            <span class="as-badge as-badge--soft">Hosting & Domain</span>
          </div>
        </AsCardSection>
        <AsCardSection>
          <div class="as-height-75">
            <p class="as-text-14 as-color-secondary-2">
              Tentukan nama domain baru dan berbagai pilihan ekstensi domain
              dengan harga terjangkau
            </p>
          </div>
        </AsCardSection>
        <AsCardSection class="as-mt-16">
          <AsButton anchor href="#" primary>Order Sekarang</AsButton>
        </AsCardSection>
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

<style lang="scss" scoped>
.as-order-product-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 20rem;
    height: auto;
  }
}
</style>
