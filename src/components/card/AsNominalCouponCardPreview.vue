<template>
  <div class="row">
    <div class="as-nominal-coupon-card">
      <AsCard border>
        <AsCardContainer sm>
          <AsCardSection flex class="gap-3">
            <img
              src="~assets/images/product-icon/niaga-point.svg"
              alt="niaga point icon"
              class="as-width-24"
            />
            <AsCardSection>
              <p class="as-text-16-semibold as-color-primary as-mb-4">
                Rp 100.000,00
              </p>
              <p class="as-text-14 as-color-secondary-2">10000 Poin</p>
            </AsCardSection>
          </AsCardSection>
        </AsCardContainer>
      </AsCard>
    </div>

    <div class="as-nominal-coupon-card">
      <AsCard border disabled>
        <AsCardContainer sm>
          <AsCardSection flex class="gap-3">
            <img
              src="~assets/images/product-icon/niaga-point.svg"
              alt="niaga point icon"
              class="as-width-24"
            />
            <AsCardSection>
              <p class="as-text-16-semibold as-color-primary as-mb-4">
                Rp 100.000,00
              </p>
              <p class="as-text-14 as-color-secondary-2">10000 Poin</p>
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
</script>

<style lang="scss" scoped>
.as-nominal-coupon-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 15.5rem;
    height: auto;
  }
}
</style>
