<template>
  <div class="col-md-8">
    <AsCard border noShadow class="as-border-radius-16">
      <AsCardContainer>
        <div class="row">
          <div class="col-md-4">
            <p class="as-text-14 as-color-secondary-2 as-mb-24">
              Nomor Virtual Account
            </p>
            <p class="as-text-14 as-color-secondary-2">Nominal Tagihan</p>
          </div>
          <div class="col-md-4">
            <p class="as-text-14-semibold as-mb-24">11366101852534</p>
            <p class="as-text-14-semibold">Rp 849.558,00</p>
          </div>
          <div class="col-md-4">
            <img
              src="~assets/images/logo/bca.svg"
              class="img-fluid"
              loading="lazy"
              alt="image"
            />
          </div>
        </div>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
</script>
