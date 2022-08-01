<template>
  <div class="row">
    <div class="as-coupon-card">
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
          <h2 class="as-text-16-bold as-mt-16">
            Kupon Diskon Perpanjangan 20% Cloud Hosting & VPS
          </h2>
          <AsCardSection class="as-mt-16">
            <div class="d-flex gap-2 as-mb-8">
              <AsBadge soft icon class="flex-fill"
                ><i class="as-icon-sync as-color-blue"></i
                ><span>Perpanjangan</span></AsBadge
              >
              <AsBadge soft icon class="flex-fill"
                ><i class="as-icon-server-double as-color-blue"></i
                ><span>Cloud VPS</span></AsBadge
              >
            </div>
            <div class="d-flex gap-2">
              <AsBadge soft icon class="flex-fill"
                ><i class="as-icon-setting as-color-blue"></i
                ><span>Cloud Hosting</span></AsBadge
              >
              <AsBadge soft icon class="flex-fill"
                ><i class="as-icon-setting as-color-blue"></i
                ><span>VPS KVM</span></AsBadge
              >
            </div>
          </AsCardSection>
        </AsCardContainer>

        <AsCardSection top>
          <AsCardContainer xsm>
            <AsCardSection
              flex
              class="d-flex align-items-center justify-content-between as-mb-16 as-mt-4"
            >
              <p class="as-text-12 as-color-secondary-2">Berlaku Hingga</p>
              <p class="as-text-12 as-color-blue">2 Hari 23 Jam</p>
            </AsCardSection>
          </AsCardContainer>
        </AsCardSection>
      </AsCard>
    </div>

    <div class="as-coupon-card">
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
          <h2 class="as-text-16-bold as-mt-16">
            Kupon Diskon Perpanjangan 20% Cloud Hosting & VPS
          </h2>
          <AsCardSection class="as-mt-16">
            <div class="d-flex gap-2 as-mb-8">
              <AsBadge soft icon class="flex-fill"
                ><i class="as-icon-sync as-color-blue"></i
                ><span>Perpanjangan</span></AsBadge
              >
              <AsBadge soft icon class="flex-fill"
                ><i class="as-icon-server-double as-color-blue"></i
                ><span>Cloud VPS</span></AsBadge
              >
            </div>
            <div class="d-flex gap-2">
              <AsBadge soft icon class="flex-fill"
                ><i class="as-icon-setting as-color-blue"></i
                ><span>Cloud Hosting</span></AsBadge
              >
              <AsBadge soft icon class="flex-fill"
                ><i class="as-icon-setting as-color-blue"></i
                ><span>VPS KVM</span></AsBadge
              >
            </div>
          </AsCardSection>
        </AsCardContainer>

        <AsCardSection top>
          <AsCardContainer xsm>
            <AsCardSection
              flex
              class="d-flex align-items-center justify-content-between as-mb-16 as-mt-4"
            >
              <p class="as-text-12 as-color-secondary-2">Berlaku Hingga</p>
              <p class="as-text-12 as-color-blue">2 Hari 23 Jam</p>
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
</script>

<style lang="scss" scoped>
.as-coupon-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 15.5rem;
    height: auto;
  }
}
</style>
