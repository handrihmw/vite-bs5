<template>
  <p class="as-color-secondary as-mb-16">Use the <code>.as-input</code> class</p>
  <div class="col-md-6">
    <AsInput
      type="text"
      id="inputText"
      data-lpignore="true"
      aria-describedby="inputHelpBlock"
      placeholder="Default text input"
    />
  </div>

  <div class="col-md-6 as-mt-24">
    <label for="inputEmail" class="as-text-16-semibold as-mb-8"
      >Email address</label
    >
    <AsInput
      type="email"
      id="inputEmail"
      data-lpignore="true"
      aria-describedby="inputHelpBlock"
      placeholder="Email input with label & info"
    />
    <span id="inputHelpBlock" class="as-info as-info--success">
      We'll never share your email with anyone else.
    </span>
  </div>

  <p class="as-color-secondary as-mb-16 as-mt-24">
    Use the <code>.as-input, .as-input--disable</code> classes
  </p>
  <div class="col-md-6">
    <AsInput
      type="text"
      id="inputText"
      disabled
      data-lpignore="true"
      aria-describedby="inputHelpBlock"
      placeholder="Default text input disabled state"
    />
  </div>
</template>

<script setup>
import AsInput from "./AsInput.vue";
</script>
