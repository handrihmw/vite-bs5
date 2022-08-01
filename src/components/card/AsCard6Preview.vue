<template>
  <div class="col-md-4">
    <AsCard white>
      <AsCardContainer>
        <img
          src="~assets/images/product-icon/checklist-circle.svg"
          class="as-width-54 as-height-54 as-mb-24"
          loading="lazy"
          alt="image"
        />
        <p class="as-text-16-semibold as-color-secondary as-mb-8">
          Masa aktif layanan
        </p>
        <div class="as-height-120">
          <h5 class="as-text-20-bold as-mb-8">8 Bulan 4 Minggu</h5>
          <p class="as-text-14 as-color-secondary">
            Layanan Anda aktif hingga 23 Februari 2023
          </p>
        </div>
        <AsCardSection>
          <AsButton anchor href="#" primary withIcon
            ><span>Perpanjang Layanan</span> <i class="as-icon-arrow-right"></i
          ></AsButton>
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
