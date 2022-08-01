<template>
  <li class="slider-card">
    <div class="slider-card__indicator">
      <span
        ><img
          src="~assets/images/samples/organism/icon-progress.svg"
          alt="icon"
      /></span>
      <hr />
    </div>

    <h3 class="slider-card__title as-text-20-bold">Online Application</h3>
    <p class="slider-card__description as-text-16">
      Apply through our Career Page or external job portals that’s officially
      posted by Niagahoster.
    </p>
  </li>
</template>

<script setup></script>

<style lang="scss" scoped>
@use "@/assets/scss/mixins/breakpoint" as *;

.slider-card {
  max-width: 20rem;
  flex-shrink: 0;
  color: var(--as-color-primary);
  list-style-type: none;

  @include screen(desktop) {
    max-width: 20.875rem;
  }

  &__indicator {
    margin-bottom: 2.375rem;
    flex-shrink: 0;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: start;

    hr {
      width: 100%;
      border: 2px solid var(--as-color-blue);
      opacity: 1;
      transform: translateY(0.1rem);
    }
  }

  &__title {
    font-size: 1.25rem;
    font-weight: 700;
    line-height: 1.625rem;
    letter-spacing: 0.005rem;
    margin-bottom: 1.125rem;
    margin-right: 3rem;
  }

  &__description {
    font-size: 1rem;
    line-height: 1.5rem;
    letter-spacing: 0.005rem;
    color: #546071;
    margin-right: 3rem;
  }
}
</style>
