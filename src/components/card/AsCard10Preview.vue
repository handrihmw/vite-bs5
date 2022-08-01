<template>
  <div class="col-md-6">
    <AsCard>
      <AsCardBackground cpanel>
        <AsCardContainer flex>
          <AsCardSection lg>
            <h2 class="as-text-24-bold as-mb-24">
              Upload Website ke File Manager
            </h2>
            <p class="as-text-12 as-color-secondary-2 as-mb-32">
              Jika Anda telah membuat website dengan coding manual dan/atau
              ingin melakukan upload file atau media melalui cPanel, silahkan
              klik disini untuk membuka File Manager
            </p>
            <AsCardSection>
              <AsButton primary sm withIcon>
                <span>Buka File Manager</span
                ><i class="as-icon-arrow-right"></i>
              </AsButton>
            </AsCardSection>
          </AsCardSection>
        </AsCardContainer>
      </AsCardBackground>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardBackground from "./AsCardBackground.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardSection from "./AsCardSection.vue";

import AsButton from "../button/AsButton.vue";
</script>
