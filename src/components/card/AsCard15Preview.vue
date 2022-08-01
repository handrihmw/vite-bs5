<template>
  <div class="col-md-4">
    <AsCard>
      <AsCardHeader>
        <div class="d-flex justify-content-between align-items-center">
          <h2 class="as-text-24-bold">Akun cPanel</h2>
          <i class="as-icon-ask-rounded as-icon-gray"></i>
        </div>
      </AsCardHeader>
      <AsCardContainer>
        <AsCardSection>
          <div class="d-flex justify-content-between as-mb-24">
            <p class="as-text-14 as-color-secondary">Username cPanel</p>
            <p class="as-text-14-semibold">u1569768</p>
          </div>
          <div class="d-flex justify-content-between">
            <p class="as-text-14 as-color-secondary">Password cPanel</p>
            <p class="as-text-14-semibold">********</p>
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
