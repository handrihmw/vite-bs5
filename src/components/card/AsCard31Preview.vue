<template>
  <div class="col-md-12">
    <AsCard>
      <AsCardHeader md>
        <h3 class="as-text-24-bold as-color-primary as-mb-16">Layanan Anda</h3>
        <p class="as-text-18-semibold as-color-secondary-2">
          Semua layanan yang telah anda beli akan ditampilkan di sini.
        </p>
      </AsCardHeader>
      <AsCardContainer fullCol>
        <AsCardSection center>
          <div
            class="pre-content pre-content__sm w-100 d-grid align-content-center"
          >
            <p class="as-text-24-semibold">Content Here</p>
          </div>
        </AsCardSection>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardHeader from "./AsCardHeader.vue";
import AsCardSection from "./AsCardSection.vue";
</script>

<style lang="scss" scoped>
@use "../../assets/scss/mixins/breakpoint" as *;

@include screen(mobileSmall) {
  .content {
    height: 500px;
  }
}

@include screen(tablet) {
  .content {
    height: 1400px;
  }
}
</style>
