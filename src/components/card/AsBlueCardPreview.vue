<template>
  <div class="as-blue-card">
    <AsCard gradientBlue>
      <AsCardContainer xlg>
        <AsCardSection>
          <img
            src="~assets/images/product-icon/server-circle.svg"
            class="as-width-64 as-height-64 as-mb-24"
            loading="lazy"
            alt="image"
          />
          <h2 class="as-text-20-bold as-mb-16">
            Ada fitur yang kurang dari layanan ini?
          </h2>
          <p class="as-text-14 as-mb-24">
            Jika ada fitur yang kurang dari layanan ini, Anda bisa melakukan
            request dengan klik tombol dibawah ini
          </p>
        </AsCardSection>
        <AsCardSection>
          <AsButton primary withIcon>
            <span>Masuk ke Cyberpanel</span><i class="as-icon-arrow-right"></i>
          </AsButton>
        </AsCardSection>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardSection from "./AsCardSection.vue";

import AsButton from "../button/AsButton.vue";
</script>

<style lang="scss" scoped>
.as-blue-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: max-content;
    height: auto;
  }
}
</style>
