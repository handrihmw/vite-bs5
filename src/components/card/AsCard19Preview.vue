<template>
  <div class="col-md-4">
    <AsCard soft center>
      <AsCardContainer>
        <AsCardSection center>
          <AsButtonIcon anchor href="#" secondary class="as-mb-24">
            <i class="as-icon-arrow-right"></i>
          </AsButtonIcon>
          <p class="as-text-16-semibold">Lihat Course Lainnya</p>
        </AsCardSection>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardSection from "./AsCardSection.vue";
import AsButtonIcon from "../button/AsButtonIcon.vue";
</script>
