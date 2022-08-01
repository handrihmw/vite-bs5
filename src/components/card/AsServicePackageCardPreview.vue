<template>
  <div class="row">
    <div class="as-service-package-card">
      <AsCard border center>
        <AsCardHeader service>
          <h2 class="as-text-16-bold">Package</h2>
        </AsCardHeader>
        <AsCardContainer sm>
          <p class="as-text-12">Rp. 10.000/bulan</p>
        </AsCardContainer>
      </AsCard>
    </div>

    <div class="as-service-package-card">
      <AsCard border center disabled>
        <AsCardHeader service>
          <h2 class="as-text-16-bold">Package</h2>
        </AsCardHeader>
        <AsCardContainer sm>
          <p class="as-text-12">Rp. 10.000/bulan</p>
        </AsCardContainer>
      </AsCard>
    </div>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardHeader from "./AsCardHeader.vue";
</script>

<style lang="scss" scoped>
.as-service-package-card {
  width: auto;
  height: auto;

  .as-card {
    max-width: max-content;
    height: auto;
    cursor: pointer;
    -webkit-box-align: baseline;

    &:focus {
      background: var(--as-gradient-blue);
      color: var(--as-color-white);
      box-shadow: none;
    }
  }
}
</style>
