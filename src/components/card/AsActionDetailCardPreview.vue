<template>
  <div class="as-action-detail-card as-mb-24">
    <AsCard gray class="as-border-radius-8">
      <AsCardContainer flex sm>
        <AsCardSection flex class="gap-3">
          <img src="~assets/images/banner/cpanel-circle.svg" />
          <div>
            <h2 class="as-text-20-bold as-mb-8">Lihat semua fitur cPanel</h2>
            <p class="as-text-16 as-color-secondary">
              Masuk ke cPanel untuk mangakses fitur cPanel selengkapnya
            </p>
          </div>
        </AsCardSection>
        <AsButtonIcon primary>
          <i class="as-icon-arrow-right"></i>
        </AsButtonIcon>
      </AsCardContainer>
    </AsCard>
  </div>

  <div class="as-action-detail-card">
    <AsCard yellow noShadow class="as-border-radius-8">
      <AsCardContainer>
        <div class="row">
          <div class="col-md-1">
            <i class="as-icon-info as-icon-orange as-icon-lg"></i>
          </div>
          <div class="col-md-11">
            <h2 class="as-text-14-semibold as-mb-8">
              Lihat semua fitur cPanel
            </h2>
            <p class="as-text-12 as-color-secondary">
              Masuk ke cPanel untuk mangakses fitur cPanel selengkapnya
            </p>
          </div>
        </div>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardSection from "./AsCardSection.vue";
import AsButtonIcon from "../button/AsButtonIcon.vue";
</script>

<style lang="scss" scoped>
.as-action-detail-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 42.625em;
    height: auto;
  }
}
</style>
