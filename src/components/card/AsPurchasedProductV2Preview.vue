<template>
  <div class="as-purchased-product-card-v2">
    <AsCard border noShadow>
      <AsCardContainer sm class="d-flex gap-5">
        <AsCardSection>
          <AsCardImage
            class="as-border-radius-8 as-width-120 as-height-80"
            loading="lazy"
          />
        </AsCardSection>
        <AsCardSection
          flex
          class="justify-content-between align-items-center w-100 as-my-8 flex-wrap"
        >
          <div>
            <h5 class="as-text-24-bold as-mb-8">yourdomain.com</h5>
            <AsBadge sm black>Domain</AsBadge>
          </div>
          <div>
            <AsCardSection flex class="gap-2 as-pt-8 as-mb-16">
              <i class="as-icon-info as-icon-gray"></i>
              <p class="as-text-12 as-color-secondary-2 as-my-8">
                Status Layanan
              </p>
              <AsBadge orange rounded>Active</AsBadge>
            </AsCardSection>
            <AsCardSection flex class="gap-2">
              <i class="as-icon-calendar as-icon-gray"></i>
              <p class="as-text-12 as-color-secondary-2">Sisa masa aktif</p>
              <p class="as-text-12-semibold as-color-primary">
                2 tahun 10 bulan
              </p>
            </AsCardSection>
          </div>
          <div class="align-self-start">
            <AsButton primary sm>Kelola Layanan</AsButton>
          </div>
        </AsCardSection>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardImage from "./AsCardImage.vue";
import AsCardSection from "./AsCardSection.vue";

import AsButton from "../button/AsButton.vue";
import AsBadge from "../badge/AsBadge.vue";
</script>

<style lang="scss" scoped>
.as-purchased-product-card-v2 {
  width: auto;
  height: auto;

  .as-card {
    max-width: 100%;
    height: auto;
  }
}
</style>
