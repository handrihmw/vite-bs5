<template>
  <div class="row">
    <div class="as-plugin-card">
      <AsCard border>
        <AsCardContainer md>
          <AsCardSection flex class="justify-content-between flex-wrap">
            <img
              src="~assets/images/samples/plugin-img.svg"
              class="img-fluid"
            />
            <AsButtonOutline sm withIcon>
              <i class="as-icon-plus"></i>
              <span>Install</span>
            </AsButtonOutline>
          </AsCardSection>
          <AsCardSection class="as-mt-24">
            <h2 class="as-text-16-bold as-color-primary as-mt-8">
              WP Mail SMTP
            </h2>
            <AsCardSection
              flex
              class="align-items-center gap-1 as-mt-8 flex-wrap"
            >
              <AsBadge sm light>Softaculous</AsBadge>
              <i class="as-icon-dot as-color-divider"></i>
              <p class="as-text-12-semibold as-color-secondary-2">v10.2.5</p>
              <i class="as-icon-dot as-color-divider"></i>
              <div class="d-flex align-items-center flex-wrap gap-1">
                <i class="as-text-12 as-icon-star as-icon-orange"></i>
                <p class="as-text-12-semibold as-color-orange">4,5</p>
              </div>
            </AsCardSection>
          </AsCardSection>
        </AsCardContainer>
      </AsCard>
    </div>

    <div class="as-plugin-card">
      <AsCard border disabled>
        <AsCardContainer md>
          <AsCardSection flex class="justify-content-between flex-wrap">
            <img
              src="~assets/images/samples/plugin-img.svg"
              class="img-fluid"
            />
            <AsButtonOutline sm withIcon>
              <i class="as-icon-plus"></i>
              <span>Install</span>
            </AsButtonOutline>
          </AsCardSection>
          <AsCardSection class="as-mt-24">
            <h2 class="as-text-16-bold as-color-primary as-mt-8">
              WP Mail SMTP
            </h2>
            <AsCardSection
              flex
              class="align-items-center gap-1 as-mt-8 flex-wrap"
            >
              <AsBadge sm light>Softaculous</AsBadge>
              <i class="as-icon-dot as-color-divider"></i>
              <p class="as-text-12-semibold as-color-secondary-2">v10.2.5</p>
              <i class="as-icon-dot as-color-divider"></i>
              <div class="d-flex align-items-center flex-wrap gap-1">
                <i class="as-text-12 as-icon-star as-icon-orange"></i>
                <p class="as-text-12-semibold as-color-orange">4,5</p>
              </div>
            </AsCardSection>
          </AsCardSection>
        </AsCardContainer>
      </AsCard>
    </div>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardSection from "./AsCardSection.vue";

import AsButtonOutline from "../button/AsButtonOutline.vue";
import AsBadge from "../badge/AsBadge.vue";
</script>

<style lang="scss" scoped>
.as-plugin-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 15.5rem;
    height: auto;
  }
}
</style>
