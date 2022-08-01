<template>
  <div class="d-flex gap-4 flex-wrap">
    <div class="as-course-card">
      <a href="">
        <AsCard white class="as-border-radius-16">
          <AsCardContainer thumb>
            <AsCardImage top loading="lazy" />
            <AsCardPlay>
              <img
                fluid
                src="~assets/images/product-icon/play-button.svg"
                class="as-width-50"
                alt="play icon"
                loading="lazy"
              />
            </AsCardPlay>
          </AsCardContainer>
          <AsCardContainer sm>
            <h3 class="as-text-18-bold as-mb-16">
              Mengenal Lebih Jauh Tentang cPanel
            </h3>
            <AsCardSection top flex class="gap-3 as-pt-16">
              <img
                src="~assets/images/product-icon/profile.svg"
                class="as-width-42 as-height-42"
                loading="lazy"
                alt="image"
              />
              <div>
                <h2 class="as-text-14-bold">Akrilvha D Wiervi</h2>
                <p class="as-text-12 as-color-secondary-2 as-mt-4">
                  Product Manager at Niagahoster
                </p>
              </div>
            </AsCardSection>
            <AsCardSection class="as-mt-24">
              <AsButton anchor href="#" primary>Ikuti Course</AsButton>
            </AsCardSection>
          </AsCardContainer>
        </AsCard>
      </a>
    </div>

    <div class="as-course-card">
      <a href="">
        <AsCard border class="as-border-radius-16">
          <AsCardContainer thumb>
            <AsCardImage top loading="lazy" />
            <AsCardPlay>
              <img
                fluid
                src="~assets/images/product-icon/play-button.svg"
                class="as-width-50"
                alt="play icon"
                loading="lazy"
              />
            </AsCardPlay>
          </AsCardContainer>
          <AsCardContainer sm>
            <h3 class="as-text-18-bold as-mb-16">
              Mengenal Lebih Jauh Tentang cPanel
            </h3>
            <AsCardSection top flex class="gap-3 as-pt-16">
              <img
                src="~assets/images/product-icon/profile.svg"
                class="as-width-42 as-height-42"
                loading="lazy"
                alt="image"
              />
              <div>
                <h2 class="as-text-14-bold">Akrilvha D Wiervi</h2>
                <p class="as-text-12 as-color-secondary-2 as-mt-4">
                  Product Manager at Niagahoster
                </p>
              </div>
            </AsCardSection>
            <AsCardSection class="as-mt-24">
              <AsButton anchor href="#" primary>Ikuti Course</AsButton>
            </AsCardSection>
          </AsCardContainer>
        </AsCard>
      </a>
    </div>

    <div class="as-course-card">
      <a href="">
        <AsCard white class="as-border-radius-16">
          <AsCardContainer thumb>
            <AsCardImage top loading="lazy" />
            <AsCardPlay>
              <img
                fluid
                src="~assets/images/product-icon/play-button.svg"
                class="as-width-50"
                alt="play icon"
                loading="lazy"
              />
            </AsCardPlay>
          </AsCardContainer>
          <AsCardContainer sm>
            <h3 class="as-text-18-bold as-mb-16">
              Mengenal Lebih Jauh Tentang cPanel
            </h3>
            <AsCardSection top flex class="gap-3 as-pt-16">
              <img
                src="~assets/images/product-icon/profile.svg"
                class="as-width-42 as-height-42"
                loading="lazy"
                alt="image"
              />
              <div>
                <h2 class="as-text-14-bold">Akrilvha D Wiervi</h2>
                <p class="as-text-12 as-color-secondary-2 as-mt-4">
                  Product Manager at Niagahoster
                </p>
              </div>
            </AsCardSection>
          </AsCardContainer>
        </AsCard>
      </a>
    </div>

    <div class="as-course-card">
      <a href="">
        <AsCard border class="as-border-radius-16">
          <AsCardContainer thumb>
            <AsCardImage top loading="lazy" />
            <AsCardPlay>
              <img
                fluid
                src="~assets/images/product-icon/play-button.svg"
                class="as-width-50"
                alt="play icon"
                loading="lazy"
              />
            </AsCardPlay>
          </AsCardContainer>
          <AsCardContainer sm>
            <h3 class="as-text-18-bold as-mb-16">
              Mengenal Lebih Jauh Tentang cPanel
            </h3>
            <AsCardSection top flex class="gap-3 as-pt-16">
              <img
                src="~assets/images/product-icon/profile.svg"
                class="as-width-42 as-height-42"
                loading="lazy"
                alt="image"
              />
              <div>
                <h2 class="as-text-14-bold">Akrilvha D Wiervi</h2>
                <p class="as-text-12 as-color-secondary-2 as-mt-4">
                  Product Manager at Niagahoster
                </p>
              </div>
            </AsCardSection>
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
import AsCardSection from "./AsCardSection.vue";
import AsCardPlay from "./AsCardPlay.vue";
import AsCardLabel from "./AsCardLabel.vue";

import AsButton from "../button/AsButton.vue";
</script>

<style lang="scss" scoped>
.as-course-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: 15.9375rem;
    height: auto;
  }
}
</style>
