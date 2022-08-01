<template>
  <p class="as-color-secondary as-mb-16">
    Use the <code>.as-input__group, .as-input__group--left</code> classes
  </p>
  <div class="col-md-6 as-mb-24">
    <AsInputGroup>
      <AsInput
        groupInput
        groupLeft
        type="text"
        id="inputDirLeft"
        placeholder="Contoh: ns1, ns2, ns3"
      />
      <AsInputGroupText left> .niagahoster.design </AsInputGroupText>
    </AsInputGroup>
  </div>

  <div class="col-md-6 as-mb-24">
    <div class="as-mb-16">
      <label for="inputDirLeft" class="as-text-16-semibold as-mb-8"
        >Childnameserver 1</label
      >
      <AsInputGroup>
        <AsInput
          groupInput
          groupLeft
          type="text"
          id="inputDirLeft"
          placeholder="Contoh: ns1, ns2, ns3"
        />
        <AsInputGroupText left> .niagahoster.design </AsInputGroupText>
      </AsInputGroup>
      <span id="idirectoryHelp" class="as-info as-info--danger as-mb-8">
        You don’t have permission to access.
      </span>
    </div>
  </div>

  <p class="as-color-secondary as-mb-16">
    Use the
    <code>.as-input__group, .as-input__group--left, .as-input--disable</code>
    classes
  </p>
  <div class="col-md-6 as-mb-24">
    <AsInputGroup>
      <AsInput
        groupInput
        groupLeft
        disabled
        type="text"
        id="inputDirLeft"
        placeholder="Contoh: ns1, ns2, ns3"
      />
      <AsInputGroupText left> .niagahoster.design </AsInputGroupText>
    </AsInputGroup>
  </div>
</template>

<script setup>
import AsInputGroup from "./AsInputGroup.vue";
import AsInputGroupText from "./AsInputGroupText.vue";
import AsInput from "./AsInput.vue";
</script>
