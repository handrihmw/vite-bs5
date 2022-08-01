<template>
  <div class="as-top-request-card">
    <AsCard white noShadow>
      <AsCardContainer
        flex
        xsm
        class="as-pt-24 as-pb-24 gap-3 align-items-center"
      >
        <AsCardSection
          center
          class="as-background-blue-light as-p-8 as-border-radius-8"
        >
          <img
            src="~assets/images/samples/icon-topRequest.svg"
            class="as-mb-8 as-width-24"
            loading="lazy"
            alt="image"
          />
          <p class="as-text-12-semibold as-color-blue-darken">9.999</p>
        </AsCardSection>
        <AsCardSection>
          <h6 class="as-text-20-bold as-mb-8">Bantuan Instalasi Panel VPS</h6>
          <p class="as-text-14-secondary-2">
            Layanan bantuan instalasi VPS, migrasi shared hosting ke VPS dan
            bantuan vps secara general (terbatas)
          </p>
        </AsCardSection>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardSection from "./AsCardSection.vue";
</script>

<style lang="scss" scoped>
.as-top-request-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: max-content;
    height: auto;
  }
}
</style>
