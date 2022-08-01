<template>
  <p class="as-color-secondary as-mb-16">
    Use the <code>.as-input, .as-input__password</code> classes
  </p>
  <div class="col-md-6">
    <AsInputPassword placeholder="Deafult input password" required />
  </div>

  <div class="col-md-6 as-mt-24">
    <div class="as-mb-8">
      <label for="inputPassword" class="as-text-16-semibold as-mb-8"
        >Password</label
      >
      <AsInputPassword
        placeholder="Input password with label & info"
        required
      />
      <span id="passwordHelpBlock" class="as-info as-info--danger">
        Your password must be 8-20 characters long, contain letters and numbers.
      </span>
    </div>
  </div>

  <p class="as-color-secondary as-mb-16 as-mt-24">
    Use the
    <code>.as-input, .as-input--disable, .as-input__password</code> classes
  </p>
  <div class="col-md-6">
    <AsInputPassword
      disabled
      placeholder="Input password disabled state"
      required
    />
  </div>
</template>

<script setup>
import AsInputPassword from "./AsInputPassword.vue";
</script>
