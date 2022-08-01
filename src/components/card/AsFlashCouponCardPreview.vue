<template>
  <div class="row">
    <div class="as-flash-coupon-card">
      <AsCard border>
        <AsCardContainer xsm>
          <AsCardContainer thumb>
            <img
              src="~assets/images/samples/coupon.svg"
              alt="coupon thumbnail"
              class="w-100"
              loading="lazy"
            />
          </AsCardContainer>
          <AsCardSection class="as-mt-16 as-mb-8">
            <AsBadge soft icon
              ><i class="as-icon-refresh as-color-blue"></i
              ><span class="as-text-14-semibold">Renewal</span></AsBadge
            >
          </AsCardSection>
          <AsCardSection flex class="gap-2">
            <img
              src="~assets/images/product-icon/niaga-point.svg"
              alt="niaga point icon"
            />
            <p class="as-text-14-semibold as-color-primary">
              2.500 Poin
              <span class="as-text-12 as-color-secondary-2">
                <del>5.000 Poin</del>
              </span>
            </p>
          </AsCardSection>
        </AsCardContainer>

        <AsCardSection top>
          <AsCardContainer xsm>
            <AsCardSection class="as-mb-8 as-mt-4">
              <p class="as-text-12 as-color-secondary as-mb-8">
                Tersedia 28 Kupon
              </p>
              <AsProgress>
                <AsProgressBar
                  valuenow="20"
                  valuemin="0"
                  valuemax="100"
                ></AsProgressBar>
              </AsProgress>
            </AsCardSection>
          </AsCardContainer>
        </AsCardSection>
      </AsCard>
    </div>

    <div class="as-flash-coupon-card">
      <AsCard border disabled>
        <AsCardContainer xsm>
          <AsCardContainer thumb>
            <img
              src="~assets/images/samples/coupon.svg"
              alt="coupon thumbnail"
              class="w-100"
              loading="lazy"
            />
          </AsCardContainer>
          <AsCardSection class="as-mt-16 as-mb-16">
            <AsBadge soft icon
              ><i class="as-icon-refresh as-color-blue"></i
              ><span class="as-text-14-semibold">Renewal</span></AsBadge
            >
          </AsCardSection>
          <AsCardSection flex class="gap-2">
            <img
              src="~assets/images/product-icon/niaga-point.svg"
              alt="niaga point icon"
            />
            <p class="as-text-14-semibold as-color-primary">
              2.500 Poin
              <span class="as-text-12 as-color-secondary-2">
                <del>5.000 Poin</del>
              </span>
            </p>
          </AsCardSection>
        </AsCardContainer>

        <AsCardSection top>
          <AsCardContainer xsm>
            <AsCardSection class="as-mb-8 as-mt-4">
              <p class="as-text-12 as-color-secondary as-mb-8">
                Tersedia 28 Kupon
              </p>
              <AsProgress>
                <AsProgressBar
                  valuenow="20"
                  valuemin="0"
                  valuemax="100"
                ></AsProgressBar>
              </AsProgress>
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

import AsBadge from "../badge/AsBadge.vue";
import AsProgress from "../progress/AsProgress.vue";
import AsProgressBar from "../progress/AsProgressBar.vue";
</script>

<style lang="scss" scoped>
.as-flash-coupon-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 15.5rem;
    height: auto;
  }
}
</style>
