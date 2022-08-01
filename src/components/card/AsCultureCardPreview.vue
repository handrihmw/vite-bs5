<template>
  <li class="section-culture__container-item">
    <div class="section-culture__container-item__overlay">
      <h3
        class="section-culture__container-item__overlay-title as-text-20-bold"
      >
        Flexible Working Hours
      </h3>
      <p
        class="section-culture__container-item__overlay-description as-text-16"
      >
        Set your working hours to fit any specific needs, without setting aside
        your responsibilities.
      </p>
    </div>
    <img src="~assets/images/samples/organism/fwh.webp" alt="pic" class="" />
  </li>
</template>

<script setup></script>

<style lang="scss">
@use "@/assets/scss/mixins/breakpoint" as *;

.section-culture__container-item {
  border-radius: 1.5rem;
  flex-shrink: 0;
  overflow: hidden;
  min-height: 21.625rem;
  width: 20rem;
  position: relative;
  list-style-type: none;

  &:hover .section-culture__container-item__overlay-title {
    transform: translateY(-10px);
  }

  &:hover .section-culture__container-item__overlay-description {
    display: block;
    opacity: 1;
  }

  &:hover .section-culture__container-item__overlay {
    height: 90%;
  }

  &__overlay {
    background: linear-gradient(180deg, rgba(18, 18, 18, 0) 0%, #121212 100%);
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    height: 50%;
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: end;
    padding-inline: 1.0625rem;
    padding-bottom: 2rem;
    transition: 0.3s;

    @include screen(desktop) {
      padding-inline: 2rem;
    }

    &-title {
      font-size: 1.25rem;
      font-weight: 700;
      line-height: 2rem;
      letter-spacing: 0.02rem;
      margin-bottom: 1.125rem;
      position: relative;
      transition: 0.5s;

      @include screen(desktop) {
        margin-bottom: unset;
      }
    }

    &-description {
      line-height: 1.5rem;
      letter-spacing: 0.005rem;
      font-size: 1rem;
      font-weight: 400;
      opacity: 1;
      transition: 0.9s;

      @include screen(desktop) {
        display: none;
        opacity: 0;
      }
    }
  }

  img {
    object-fit: cover;
    width: 100%;
    height: 100%;
  }

  @include screen(desktop) {
    min-height: 21.625rem;
    max-height: 21.625rem;
  }

  @include screen(desktop) {
    width: unset;
  }
}
</style>
