<template>
  <div class="as-mt-24">
    <div class="d-flex flex-wrap gap-2">
      <AsButtonOutline anchor href="#modalColumn">Preview</AsButtonOutline>
    </div>

    <AsModal md id="modalColumn">
      <div class="row">
        <div class="col-md-8 as-border--right">
          <AsModalHeader>
            <h5 class="as-text-24-bold">Modal Title Here</h5>
          </AsModalHeader>
          <AsModalSection>
            <div class="pre-content pre-content__md"></div>
          </AsModalSection>
        </div>
        <div class="col-md-4">
          <AsModalSection close> </AsModalSection>
          <AsModalSection>
            <div class="pre-content pre-content__sm"></div>
            <div class="as-text-center align-items-center as-pt-32">
              <AsButton primary sm>Button Label</AsButton>
            </div>
          </AsModalSection>
        </div>
      </div>
    </AsModal>
  </div>
</template>

<script setup>
import AsModal from "./AsModal.vue";
import AsModalFooter from "./AsModalFooter.vue";
import AsModalHeader from "./AsModalHeader.vue";
import AsModalSection from "./AsModalSection.vue";

import AsButtonOutline from "../button/AsButtonOutline.vue";
import AsButton from "../button/AsButton.vue";
</script>
