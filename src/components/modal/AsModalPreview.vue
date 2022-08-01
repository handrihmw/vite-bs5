<template>
  <div class="as-mt-24">
    <div class="d-flex flex-wrap gap-3">
      <AsButton anchor href="#modalDefault">Preview 1</AsButton>
      <AsButton anchor href="#modalDefault2">Preview 2</AsButton>
    </div>

    <!-- Modal Content 1 -->
    <AsModal id="modalDefault">
      <AsModalHeader close />
      <AsModalSection class="as-border--bottom">
        <h5 class="as-text-24-bold">Modal Title Here</h5>
        <p class="as-text-16-semibold">This is Sub Heading</p>
        <div class="pre-content pre-content__xs as-mt-24"></div>
      </AsModalSection>
      <AsModalSection>
        <div class="row">
          <div class="col-md-12">
            <div class="pre-content pre-content__md"></div>
          </div>
        </div>
      </AsModalSection>
      <AsModalFooter
        class="as-border--top d-flex flex-wrap gap-3 justify-content-end"
      >
        <AsButton primary sm>Button Label</AsButton>
        <AsButtonOutline primary sm>Button Label Other</AsButtonOutline>
      </AsModalFooter>
    </AsModal>

    <!-- Modal Content 2 -->
    <AsModal id="modalDefault2">
      <AsModalHeader close />
      <AsModalSection class="as-border--bottom">
        <h5 class="as-text-24-bold">Modal Title Here</h5>
        <p class="as-text-16-semibold">This is Sub Heading</p>
      </AsModalSection>
      <AsModalSection>
        <div class="row">
          <div class="col-md-12">
            <div class="pre-content pre-content__md"></div>
          </div>
        </div>
      </AsModalSection>
      <AsModalFooter
        class="as-border--top d-flex flex-wrap align-items-center justify-content-between"
      >
        <a href="#" class="as-text-14-bold as-link-red as-mb-16 text-center"
          >Text Link Danger</a
        >
        <div class="d-flex flex-wrap gap-3">
          <AsButton primary sm>Button Label</AsButton>
          <AsButtonOutline primary sm>Button Label Other</AsButtonOutline>
        </div>
      </AsModalFooter>
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

<style lang="scss" scoped>
@use "../../assets/scss/mixins/breakpoint" as *;

.as-link-red {
  margin: 0 auto;
  @include screen(desktop) {
    margin: 0;
  }
}
</style>
