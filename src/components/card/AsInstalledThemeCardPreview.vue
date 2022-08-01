<template>
  <div class="row">
    <div class="as-installed-theme-card">
      <AsCard border>
        <AsCardContainer md>
          <h2 class="as-text-16-bold as-color-primary as-mb-24">
            Twenty Nineteen Nineteen Twenty
          </h2>
          <AsCardSection class="as-mb-4">
            <AsCardImage installed class="as-border-radius-8" loading="lazy" />
          </AsCardSection>
        </AsCardContainer>
        <AsCardSection top>
          <AsCardContainer md>
            <AsCardSection flex class="justify-content-between">
              <div class="d-flex">
                <AsBadge disabled v-if="isDisabled">Tidak Aktif</AsBadge>
                <AsBadge green v-else>Aktif</AsBadge>
              </div>

              <div class="as-switch m-0">
                <input
                  type="checkbox"
                  id="toggle1"
                  @click="isDisabled = !isDisabled"
                />
                <label for="toggle1"></label>
              </div>
            </AsCardSection>
          </AsCardContainer>
        </AsCardSection>
      </AsCard>
    </div>

    <div class="as-installed-theme-card">
      <AsCard border disabled>
        <AsCardContainer md>
          <h2 class="as-text-16-bold as-color-primary as-mb-24">
            Twenty Nineteen Nineteen Twenty
          </h2>
          <AsCardSection class="as-mb-4">
            <AsCardImage installed class="as-border-radius-8" loading="lazy" />
          </AsCardSection>
        </AsCardContainer>
        <AsCardSection top>
          <AsCardContainer md>
            <AsCardSection flex class="justify-content-between">
              <div class="d-flex">
                <AsBadge disabled v-if="isDisabled">Tidak Aktif</AsBadge>
                <AsBadge green v-else>Aktif</AsBadge>
              </div>

              <div class="as-switch m-0">
                <input
                  type="checkbox"
                  id="toggle1"
                  @click="isDisabled = !isDisabled"
                />
                <label for="toggle1"></label>
              </div>
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
import AsCardImage from "./AsCardImage.vue";
import AsCardSection from "./AsCardSection.vue";

import AsBadge from "../badge/AsBadge.vue";

let isDisabled = ref(true);
</script>

<style lang="scss" scoped>
.as-installed-theme-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 21.125rem;
    height: auto;
  }
}
</style>
