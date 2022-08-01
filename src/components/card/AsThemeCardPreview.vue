<template>
  <div class="d-flex gap-4 flex-wrap">
    <div class="as-theme-card">
      <a href="#">
        <AsCard border center>
          <AsCardContainer thumb>
            <AsCardImage theme loading="lazy" />
          </AsCardContainer>
          <AsCardContainer sm>
            <h3 class="as-text-14-bold as-color-primary">Twenty Twenty-One</h3>
            <p class="as-text-12 as-color-secondary-2 text-uppercase as-my-16">
              gratis
            </p>
            <AsButton sm primary fluid> Pilih Tema </AsButton>
          </AsCardContainer>
        </AsCard>
      </a>
    </div>

    <div class="as-theme-card">
      <a href="#">
        <AsCard border center>
          <AsCardContainer thumb>
            <AsCardImage theme loading="lazy" />
          </AsCardContainer>
          <AsCardContainer sm>
            <h3 class="as-text-14-bold as-color-primary">Twenty Twenty-One</h3>
            <p class="as-text-12 as-color-secondary-2 text-uppercase as-my-16">
              gratis
            </p>
            <AsButtonOutline sm primary fluid class="as-mb-16">
              Lihat Detail Fitur
            </AsButtonOutline>
            <AsButton sm primary fluid> Pilih Tema </AsButton>
          </AsCardContainer>
        </AsCard>
      </a>
    </div>

    <div class="as-theme-card">
      <a href="#">
        <AsCard border center disabled>
          <AsCardContainer thumb>
            <AsCardImage theme loading="lazy" />
          </AsCardContainer>
          <AsCardContainer sm>
            <h3 class="as-text-14-bold as-color-primary">Twenty Twenty-One</h3>
            <p class="as-text-12 as-color-secondary-2 text-uppercase as-my-16">
              gratis
            </p>
            <AsButtonOutline sm primary fluid class="as-mb-16">
              Lihat Detail Fitur
            </AsButtonOutline>
            <AsButton sm primary fluid> Pilih Tema </AsButton>
          </AsCardContainer>
        </AsCard>
      </a>
    </div>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardImage from "./AsCardImage.vue";

import AsButton from "../button/AsButton.vue";
import AsButtonOutline from "../button/AsButtonOutline.vue";
</script>

<style lang="scss" scoped>
.as-theme-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 11.5625rem;
    height: auto;
  }
}
</style>
