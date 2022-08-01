<template>
  <div class="row">
    <div class="as-simple-coupon-card">
      <AsCard border>
        <AsCardContainer xsm>
          <AsCardContainer thumb>
            <img
              src="~assets/images/samples/kupon-bayi.png"
              alt="coupon thumbnail"
              class="w-100"
              loading="lazy"
            />
          </AsCardContainer>
          <h2 class="as-text-16-bold as-mt-16">Kupon Bayi</h2>
        </AsCardContainer>

        <AsCardSection top>
          <AsCardContainer xsm>
            <AsCardSection flex class="gap-2">
              <img
                src="~assets/images/product-icon/niaga-point.svg"
                alt="niaga point icon"
              />
              <p class="as-text-14-semibold as-color-secondary-2">
                100 - 500 poin
              </p>
            </AsCardSection>
          </AsCardContainer>
        </AsCardSection>
      </AsCard>
    </div>

    <div class="as-simple-coupon-card">
      <AsCard border disabled>
        <AsCardContainer xsm>
          <AsCardContainer thumb>
            <img
              src="~assets/images/samples/kupon-bayi.png"
              alt="coupon thumbnail"
              class="w-100"
              loading="lazy"
            />
          </AsCardContainer>
          <h2 class="as-text-16-bold as-mt-16">Kupon Bayi</h2>
        </AsCardContainer>

        <AsCardSection top>
          <AsCardContainer xsm>
            <AsCardSection flex class="gap-2">
              <img
                src="~assets/images/product-icon/niaga-point.svg"
                alt="niaga point icon"
              />
              <p class="as-text-14-semibold as-color-secondary-2">
                100 - 500 poin
              </p>
            </AsCardSection>
          </AsCardContainer>
        </AsCardSection>
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
.as-simple-coupon-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 15.5rem;
    height: auto;
  }
}
</style>
