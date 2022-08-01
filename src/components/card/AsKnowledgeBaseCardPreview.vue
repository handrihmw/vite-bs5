<template>
  <div class="row">
    <div class="as-knowledge-base-card">
      <AsCard noShadow>
        <AsCardSection flex class="gap-3 align-items-center">
          <AsCardImage class="as-border-radius-8 as-width-84 as-height-84" />
          <AsCardSection>
            <h3 class="as-text-16-bold as-mb-8">
              Cara Masuk ke Panel VPS di Member...
            </h3>
            <AsCardSection flex class="gap-1 align-items-center">
              <i class="as-icon-clock as-color-secondary-2"></i>
              <p class="as-text-12-semibold as-color-secondary-2">
                Waktu baca: 2 menit
              </p>
            </AsCardSection>
          </AsCardSection>
        </AsCardSection>
      </AsCard>
    </div>

    <div class="as-knowledge-base-card">
      <AsCard noShadow disabled>
        <AsCardSection flex class="gap-3 align-items-center">
          <AsCardImage class="as-border-radius-8 as-width-84 as-height-84" />
          <AsCardSection>
            <h3 class="as-text-16-bold as-mb-8">
              Cara Masuk ke Panel VPS di Member...
            </h3>
            <AsCardSection flex class="gap-1 align-items-center">
              <i class="as-icon-clock as-color-secondary-2"></i>
              <p class="as-text-12-semibold as-color-secondary-2">
                Waktu baca: 2 menit
              </p>
            </AsCardSection>
          </AsCardSection>
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
</script>

<style lang="scss" scoped>
.as-knowledge-base-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 18.875rem;
    height: auto;

    &:hover .as-card__section h3 {
      color: var(--as-color-blue);
    }
  }
}
</style>
