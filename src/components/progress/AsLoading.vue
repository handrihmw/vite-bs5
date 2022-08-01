<template>
  <div class="loader loader-quart"></div>
</template>

<style scoped>
.loader {
  position: relative;
  display: inline-block;
  width: 88px;
  height: 88px;
  vertical-align: middle;
}

.loader-quart {
  border-radius: 50px;
  border: 10px solid var(--as-color-soft);
}

.loader-quart:after {
  content: "";
  position: absolute;
  top: -8px;
  left: -8px;
  bottom: -8px;
  right: -8px;
  border-radius: 50px;
  border: 10px solid transparent;
  border-top-color: var(--as-color-blue-light);
  -webkit-animation: spin 1s linear infinite;
  animation: spin 1s linear infinite;
}

@-webkit-keyframes spin {
  0% {
    -webkit-transform: rotate(0deg);
    tranform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(360deg);
    tranform: rotate(360deg);
  }
}

@keyframes spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(360deg);
    transform: rotate(360deg);
  }
}
</style>
