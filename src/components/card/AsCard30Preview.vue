<template>
  <div class="col-md-6">
    <AsCard>
      <AsCardHeader md>
        <h1 class="as-text-24-bold as-color-primary">Section Title</h1>
      </AsCardHeader>
      <AsCardContainer class="as-pt-24 as-pb-24">
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
