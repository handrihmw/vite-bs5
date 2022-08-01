<template>
  <div class="row">
    <div class="as-shortcut-card as-mb-24">
      <a href="#">
        <AsCard border>
          <AsCardContainer>
            <AsCardSection center>
              <img
                src="~assets/images/product-icon/add-on.svg"
                class="as-width-54 as-height-54 as-mb-24"
                loading="lazy"
                alt="image"
              />
              <p class="as-text-14-semibold">Add-on Domain</p>
            </AsCardSection>
          </AsCardContainer>
        </AsCard>
      </a>
    </div>
  </div>

  <div class="row">
    <div class="as-shortcut-card">
      <a href="#">
        <AsCard soft dashed>
          <AsCardContainer>
            <AsCardSection center>
              <img
                src="~assets/images/product-icon/shortcut.svg"
                class="as-width-54 as-height-54 as-mb-24"
                loading="lazy"
                alt="image"
              />
              <p class="as-text-14-semibold">Atur Shortcut</p>
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
import AsCardSection from "./AsCardSection.vue";
</script>

<style lang="scss" scoped>
.as-shortcut-card {
  width: auto;
  height: auto;

  .as-card {
    width: 9.25rem;
    height: 9.25rem;
  }
}
</style>
