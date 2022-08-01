<template>
  <li class="slider-card">
    <img
      src="~assets/images/samples/organism/icon-customer-obsession.svg"
      alt="icon"
    />
    <h3 class="slider-card__title as-text-20-bold">Customer Obsession</h3>
    <ul class="slider-card__list as-text-16">
      <li>You start with the customer and work backwards</li>
      <li>
        You extensively research and strive to understand our customers better
      </li>
      <li>You work with great effort to earn and keep customer trust</li>
    </ul>
  </li>
</template>

<script setup></script>

<style lang="scss" scoped>
@use "@/assets/scss/mixins/breakpoint" as *;

.slider-card {
  max-width: 18.5rem;
  min-height: 20.5rem;
  flex-shrink: 0;
  background: white;
  box-shadow: 0px 4px 24px rgba(0, 87, 178, 0.08);
  border-radius: 1.5rem;
  padding: 2rem;
  color: var(--as-color-primary);
  list-style-type: none;

  img {
    width: 2.23125rem;
    margin-bottom: 2.125rem;
  }

  &__title {
    font-size: 1.25rem;
    font-weight: 700;
    line-height: 1.625rem;
    letter-spacing: 0.005rem;
    margin-bottom: 0.75rem;
  }

  &__list {
    list-style-type: disc;

    li {
      font-size: 1rem;
      line-height: 1.5rem;
      letter-spacing: 0.005rem;
      margin-left: 1.5rem;
      color: var(--as-color-primary);

      &::marker {
        color: var(--as-color-primary);
        font-size: 0.8rem;
      }
    }
  }
}
</style>
