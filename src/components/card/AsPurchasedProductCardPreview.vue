<template>
  <div class="as-purchased-product-card">
    <a href="#">
      <AsCard>
        <AsCardContainer thumb>
          <AsCardImage top purchased />
          <AsCardLabel>
            <AsBadge black>Paket VPS Professional</AsBadge>
          </AsCardLabel>
        </AsCardContainer>
        <AsCardContainer border sm class="as-pb-24">
          <h3 class="as-text-18-bold as-mb-16">namadomain.id</h3>
          <AsCardSection flex top class="gap-3 as-pt-8 as-mb-8">
            <i class="as-icon-info as-icon-gray"></i>
            <p class="as-text-12 as-color-secondary-2 as-my-8">
              Status Layanan
            </p>
            <AsBadge green>Active</AsBadge>
          </AsCardSection>
          <AsCardSection flex class="gap-3">
            <i class="as-icon-calendar as-icon-gray"></i>
            <p class="as-text-12 as-color-secondary-2">Aktif Hingga</p>
            <p class="as-text-12-semibold as-color-primary">2 tahun 10 bulan</p>
          </AsCardSection>
        </AsCardContainer>
      </AsCard>
    </a>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardImage from "./AsCardImage.vue";
import AsCardSection from "./AsCardSection.vue";
import AsCardLabel from "./AsCardLabel.vue";

import AsBadge from "../badge/AsBadge.vue";
</script>

<style lang="scss" scoped>
.as-purchased-product-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 15.5rem;
    height: auto;
  }
}
</style>
