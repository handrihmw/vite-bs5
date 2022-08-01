<template>
  <div class="col-md-4">
    <AsCard>
      <AsCardHeader>
        <h2 class="as-text-24-bold">Detail Hosting</h2>
      </AsCardHeader>
      <AsCardContainer>
        <AsCardSection class="as-mb-24">
          <div class="d-flex justify-content-between">
            <p class="as-text-14 as-color-secondary-2">Nameserver</p>
            <a href="#" class="as-text-14-semibold as-link">namadomain.com</a>
          </div>
        </AsCardSection>
        <AsCardSection class="as-mb-24">
          <div class="d-flex justify-content-between">
            <div class="d-flex justify-content-between gap-2">
              <p class="as-text-14 as-color-secondary-2">Nameserver</p>
              <i class="as-icon-ask-rounded as-icon-gray"></i>
            </div>
            <div>
              <div
                class="d-flex justify-content-between align-items-center gap-2 as-mb-8"
              >
                <p class="as-text-14 as-color-primary">ns1.niagahoster.com</p>
                <i class="as-icon-copy as-icon-gray"></i>
              </div>
              <div
                class="d-flex justify-content-between align-items-center gap-2"
              >
                <p class="as-text-14 as-color-primary">ns1.niagahoster.com</p>
                <i class="as-icon-copy as-icon-gray"></i>
              </div>
            </div>
          </div>
        </AsCardSection>
        <AsCardSection class="as-mb-32">
          <div class="d-flex justify-content-between">
            <p class="as-text-14 as-color-secondary-2">IP Website</p>
            <div
              class="d-flex justify-content-between align-items-center gap-2"
            >
              <p class="as-text-14 as-color-primary">109.106.252.91</p>
              <i class="as-icon-copy as-icon-gray"></i>
            </div>
          </div>
        </AsCardSection>
        <AsButtonOutline anchor href="#" primary withIcon
          ><span>Lihat detail selengkapnya</span
          ><i class="as-icon-arrow-right"></i
        ></AsButtonOutline>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardHeader from "./AsCardHeader.vue";
import AsCardSection from "./AsCardSection.vue";

import AsButtonOutline from "../button/AsButtonOutline.vue";
</script>
