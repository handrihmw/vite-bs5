<template>
  <div class="col-md-8">
    <AsCard>
      <AsCardBackground ssl>
        <AsCardContainer flex>
          <AsCardSection md>
            <h2 class="as-text-24-bold as-mb-24">
              Keamanan Website - Sertifikat SSL
            </h2>
            <p class="as-text-12 as-color-secondary-2 as-mb-32">
              Tingkatkan keamanan data dalam website Anda dengan enkripsi
              terbaru dari SSL
            </p>
            <AsCardSection>
              <AsButton primary sm withIcon>
                <i class="as-icon-plus"></i>
                <span>Beli Sertifikat SSL</span>
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
