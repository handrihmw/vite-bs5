<template>
  <div class="col-md-6">
    <AsCard>
      <AsCardBackground cms>
        <AsCardContainer flex>
          <AsCardSection lg>
            <h2 class="as-text-24-bold as-mb-24">Install dan Kelola CMS</h2>
            <p class="as-text-12 as-color-secondary-2 as-mb-32">
              Anda bisa membuat website dari CMS populer dengan segala
              kemudahannya, sehingga website Anda dapat segera online. Jika
              pernah menginstall sebelumnya, cek instalasi terlebih dahulu
            </p>
            <AsCardSection flex class="flex-wrap gap-2">
              <AsButton primary sm withIcon>
                <span>Install Sekarang</span><i class="as-icon-arrow-right"></i>
              </AsButton>
              <AsButtonOutline primary sm> Cek Instalasi </AsButtonOutline>
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
import AsButtonOutline from "../button/AsButtonOutline.vue";
</script>
