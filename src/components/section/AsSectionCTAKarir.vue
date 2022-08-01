<template>
  <section class="as-section-dark as-py-60 as-px-20">
    <img
      src="~assets/images/samples/organism/lpkarir/illust-left-culture.svg"
      class="illustration--left"
      loading="lazy"
    />
    <img
      src="~assets/images/samples/organism/lpkarir/illust-right-culture.svg"
      class="illustration--right"
      loading="lazy"
    />
    <div class="as-section__container">
      <h2 class="as-section__title as-mb-32">Niagahoster Working Culture</h2>
      <p class="as-section__description as-mb-40">
        Niagahoster has 10 underlying principles to guide Rangers in making
        smart decisions, taking measurable actions, and working towards our
        goals.
      </p>
      <button class="as-btn as-btn--lg as-btn--primary as-btn--fluid">
        See Our Principles
      </button>
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss">
@use "@/assets/scss/components/section.scss";
@use "@/assets/scss/mixins/breakpoint" as *;

.as-section-dark {
  position: relative;

  @include screen(desktop) {
    padding-block: 5.125rem;
    text-align: center;
  }

  .illustration--left,
  .illustration--right {
    position: absolute;
    top: 0;
    bottom: 0;
    max-width: 19.375rem;
    display: none;

    @include screen(desktop) {
      display: block;
    }
  }

  .illustration--left {
    left: 0;
  }
  .illustration--right {
    right: 0;
  }

  .as-section__container {
    @include screen(desktop) {
      max-width: 50rem;
      margin-inline: auto;
    }
  }

  .as-btn {
    @include screen(desktop) {
      width: unset;
      padding-inline: 4rem;
      margin-inline: auto;
    }
  }
}
</style>
