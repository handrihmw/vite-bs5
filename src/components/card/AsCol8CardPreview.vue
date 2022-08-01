<template>
  <div class="col-md-8 as-mt-32">
    <AsCard>
      <AsCardHeader md>
        <h1 class="as-text-24-bold as-color-primary as-mb-4">Section Title</h1>
        <p class="as-text-14 as-color-secondary-2 as-mt-8">
          Lorem ipsum doler sit amet Lorem ipsum doler sit amet Lorem ipsum
          doler sit amet Lorem ipsum doler sit amet Lorem ipsum doler sit amet.
        </p>
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
