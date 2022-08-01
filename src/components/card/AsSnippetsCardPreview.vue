<template>
  <li class="as-snippets-card">
    <a href="#">
      <img src="~assets/images/samples/organism/pic-1.webp" alt="pic 1" />
      <span class="overlay"></span>
    </a>
  </li>
</template>

<style lang="scss">
.as-snippets-card {
  position: relative;
  object-fit: cover;
  list-style-type: none;
  cursor: pointer;
  width: 100%;
  height: 100%;

  img {
    object-fit: cover;
    width: 100%;
    height: 100%;
  }

  .overlay {
    position: absolute;
    top: 0;
    left: 0;
    background-color: #00000080;
    height: 100%;
    width: 100%;
    z-index: 999;
    opacity: 0;
    transition: 0.5s ease;
  }

  &:hover .overlay {
    opacity: 1;
  }
}
</style>
