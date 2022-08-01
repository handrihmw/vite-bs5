<template>
  <div class="as-mt-24">
    <div class="d-flex flex-wrap gap-3">
      <AsButtonOutline anchor href="#modalCenter">Preview 1</AsButtonOutline>
      <AsButtonOutline anchor href="#modalCenter2">Preview 2</AsButtonOutline>
    </div>

    <!-- Modal Content 1 -->
    <AsModal id="modalCenter" sm>
      <AsModalHeader close> </AsModalHeader>
      <AsModalSection center>
        <div class="section-wrapper">
          <img
            src="~assets/images/illustration/success.svg"
            class="img-fluid as-mb-24"
            loading="lazy"
            alt="test"
          />
          <h4 class="as-text-18-bold as-mb-16">Message Title</h4>
          <p class="as-text-12 as-color-secondary-2">
            Lorem ipsum doler sit amet, Lorem ipsum doler sit amet, Lorem ipsum
            doler sit amet Lorem ipsum doler sit amet Lorem ipsum doler sit amet
            Lorem ipsum doler sit amet
          </p>
        </div>
      </AsModalSection>
      <AsModalFooter class="d-flex flex-wrap gap-3 justify-content-center">
        <AsButtonOutline primary sm>Button Label</AsButtonOutline>
        <AsButton primary sm>Button Label Other</AsButton>
      </AsModalFooter>
    </AsModal>

    <!-- Modal Content 2 -->
    <AsModal xs id="modalCenter2">
      <AsModalHeader close> </AsModalHeader>
      <AsModalSection center>
        <div class="section-wrapper">
          <img
            src="~assets/images/illustration/success.svg"
            class="img-fluid as-mb-24"
            loading="lazy"
            alt="test"
          />
          <h4 class="as-text-18-bold as-mb-16">Message Title</h4>
          <p class="as-text-12 as-color-secondary-2">
            Lorem ipsum doler sit amet, Lorem ipsum doler sit amet, Lorem ipsum
            doler sit amet Lorem ipsum doler sit amet Lorem ipsum doler sit amet
            Lorem ipsum doler sit amet
          </p>
        </div>
      </AsModalSection>
      <AsModalFooter class="d-flex justify-content-center">
        <AsButton primary sm>Button Label</AsButton>
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
.section-wrapper {
  @include screen(tablet) {
    width: 400px;
    margin: 0 auto;
  }
}
</style>
