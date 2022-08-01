<template>
  <div class="pre-card">
    <div class="pre-card-header">
      <h4 class="as-text-20-semibold">Rating Small</h4>
    </div>
    <div class="pre-card-body">
      <p class="as-color-secondary as-mb-24">
        Use the
        <code
          >.as-rating, .as-icon-star-outline, .as-rating--sm,
          .as-rating--two</code
        >
        classes
      </p>

      <div class="as-rating as-rating--sm as-rating--two">
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
      </div>
    </div>
  </div>

  <div class="pre-card">
    <div class="pre-card-header">
      <h4 class="as-text-20-semibold">Rating Medium</h4>
    </div>
    <div class="pre-card-body">
      <p class="as-color-secondary as-mb-24">
        Use the
        <code
          >.as-rating, .as-icon-star-outline, .as-rating--md,
          .as-rating--three-half</code
        >
        classes
      </p>

      <div class="as-rating as-rating--md as-rating--three-half">
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
      </div>
    </div>
  </div>

  <div class="pre-card">
    <div class="pre-card-header">
      <h4 class="as-text-20-semibold">Rating Large</h4>
    </div>
    <div class="pre-card-body">
      <p class="as-color-secondary as-mb-24">
        Use the
        <code
          >.as-rating, .as-icon-star-outline, .as-rating--lg,
          .as-rating--five</code
        >
        classes
      </p>

      <div class="as-rating as-rating--lg as-rating--five">
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
        <em class="as-icon-star-outline"></em>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss">
@use "@/assets/scss/components/rating.scss";
</style>
