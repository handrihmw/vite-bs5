<template>
  <div class="col-md-4">
    <AsCard white>
      <AsCardContainer>
        <AsCardSection>
          <img
            src="~assets/images/product-icon/server-circle.svg"
            class="as-width-54 as-height-54 as-mb-24"
            loading="lazy"
            alt="image"
          />
          <h2 class="as-text-24-bold as-mb-24">Kelola Hosting</h2>
          <div class="as-height-85">
            <p class="as-text-16 as-color-secondary-2">Pilih akun hosting</p>
          </div>
        </AsCardSection>
        <AsCardSection class="as-mt-24">
          <AsButton anchor href="#" primary>Kelola VPS</AsButton>
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
