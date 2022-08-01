<template>
  <div class="col-md-6">
    <AsCard class="as-border-radius-16 overflow-hidden">
      <div class="row">
        <div class="col-md-9">
          <AsCardContainer>
            <h1 class="as-text-24-bold as-color-primary">Section Title</h1>
            <p class="as-text-12 as-color-secondary-2 as-mt-16">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla
              eligendi doloremque quis nostrum pariatur iste, assumenda nemo
              laborum! Aperiam velit voluptatem beatae saepe laudantium
              voluptas?
            </p>
            <AsCardSection
              flex
              class="d-flex align-items-center gap-2 flex-wrap as-mt-24 as-pt-8"
            >
              <AsButton primary withIcon sm
                ><span>Button Label</span><i class="as-icon-arrow-right"></i
              ></AsButton>
              <AsButtonOutline primary sm>Button Label</AsButtonOutline>
            </AsCardSection>
          </AsCardContainer>
        </div>
        <AsCardSection
          left
          class="col-md-3 text-center as-p-24 d-flex align-items-center justify-content-center as-background-gray-soft"
        >
          <p class="as-text-16">Illustration/Image Here</p>
        </AsCardSection>
      </div>
    </AsCard>
  </div>
</template>

<script setup>
import AsCard from "./AsCard.vue";
import AsCardContainer from "./AsCardContainer.vue";
import AsCardSection from "./AsCardSection.vue";

import AsButton from "../button/AsButton.vue";
import AsButtonOutline from "../button/AsButtonOutline.vue";
import AsButtonIcon from "../button/AsButtonIcon.vue";
</script>
