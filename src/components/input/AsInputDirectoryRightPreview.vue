<template>
  <p class="as-color-secondary as-mb-16">
    Use the <code>.as-input__group, .as-input__group-text--right</code> classes
  </p>
  <div class="col-md-6 as-mb-24">
    <div class="as-mb-16">
      <AsInputGroup>
        <AsInputGroupText right> www.niagahoster.design </AsInputGroupText>
        <AsInput
          groupInput
          groupRight
          type="text"
          id="inputDirRight"
          placeholder="/filename"
        />
      </AsInputGroup>
    </div>
  </div>

  <div class="col-md-6 as-mb-24">
    <div class="as-mb-16">
      <label for="inputDirRight" class="as-text-16-semibold as-mb-8"
        >Choose your directory</label
      >
      <AsInputGroup>
        <AsInputGroupText right> www.niagahoster.design </AsInputGroupText>
        <AsInput
          groupInput
          groupRight
          type="text"
          id="inputDirRight"
          placeholder="/filename"
        />
      </AsInputGroup>
      <span id="idirectoryHelp" class="as-info as-info--danger as-mb-8">
        You don’t have permission to access.
      </span>
    </div>
  </div>

  <p class="as-color-secondary as-mb-16">
    Use the
    <code
      >.as-input__group, .as-input__group-text--right, .as-input--disable</code
    >
    classes
  </p>
  <div class="col-md-6 as-mb-24">
    <div class="as-mb-16">
      <AsInputGroup>
        <AsInputGroupText right> www.niagahoster.design </AsInputGroupText>
        <AsInput
          groupInput
          groupRight
          disabled
          type="text"
          id="inputDirRight"
          placeholder="/filename"
        />
      </AsInputGroup>
    </div>
  </div>
</template>

<script setup>
import AsInputGroup from "./AsInputGroup.vue";
import AsInputGroupText from "./AsInputGroupText.vue";
import AsInput from "./AsInput.vue";
</script>
