<template>
  <div class="col-md-3">
    <AsCard white center>
      <AsCardContainer lg>
        <AsCardSection center>
          <div
            class="pre-content pre-content__sm w-100 d-grid align-content-center"
          >
            <p class="as-text-24-semibold">Content Here</p>
          </div>
        </AsCardSection>
        <AsCardSection class="as-mt-32">
          <AsButton anchor href="#" primary fluid class="as-mt-4"
            >Order Sekarang</AsButton
          >
        </AsCardSection>
      </AsCardContainer>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardSection from "./AsCardSection.vue";
import AsButton from "../button/AsButton.vue";
</script>
