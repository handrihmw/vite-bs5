<template>
  <AsBanner src="https://source.unsplash.com/1600x900/?nature,water">
    <div class="as-banner__container">
      <div class="as-banner__overlay">
        <div class="as-banner__wrapper">
          <div class="as-banner__content">
            <h2 class="as-text-28-bold as-mb-16">Apa saja asalkan halal</h2>
            <p class="as-text-16 as-mb-24">
              Perkuat bisnis anda dengan memiliki website. Gunakan kesempatan
              promo ini untuk bisa mendapatkan website impian anda!
            </p>
            <AsButton primary withIcon>
              <span>Install Sekarang</span><i class="as-icon-arrow-right"></i>
            </AsButton>
          </div>
        </div>
      </div>
    </div>
  </AsBanner>
</template>

<script setup>
import AsBanner from "./AsBanner.vue";
import AsButton from "../button/AsButton.vue";
</script>
