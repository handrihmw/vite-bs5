<template>
  <p class="as-color-secondary as-mb-16">
    Use the <code>.as-textarea</code> class
  </p>
  <div class="col-md-6 as-mb-24">
    <AsInputTextArea
      class="as-text-14"
      modelValue="Masukkan body atau konten email yang ingin Anda kirimkan secara otomatis"
    />
  </div>
  <div class="col-md-6 as-mb-24">
    <label for="inputEmail" class="as-text-16-semibold as-mb-8"
      >Body Email</label
    >
    <AsInputTextArea
      class="as-text-14"
      modelValue="Masukkan body atau konten email yang ingin Anda kirimkan secara otomatis"
    />
    <span id="inputHelpBlock" class="as-info as-info--success as-mb-8">
      We'll never share your email with anyone else.
    </span>
  </div>
  <p class="as-color-secondary as-mb-16">
    Use the <code>.as-textarea, .as-textarea--disable</code> class
  </p>
  <div class="col-md-6 as-mb-24">
    <AsInputTextArea
      class="as-text-14"
      modelValue="Masukkan body atau konten email yang ingin Anda kirimkan secara otomatis"
      disabled
    />
  </div>
</template>

<script setup>
import AsInputTextArea from "./AsInputTextArea.vue";
</script>
