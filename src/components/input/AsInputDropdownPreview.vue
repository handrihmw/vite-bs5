<template>
  <div class="col-md-6 as-mb-24">
    <AsInputGroup>
      <AsInput
        groupInput
        groupLeft
        type="text"
        id="inputDir"
        placeholder="no-reply"
      />
      <AsInputDropdown text="niagahoster.design">
        <AsDropdownMenuItem>Lorem ipsum</AsDropdownMenuItem>
        <AsDropdownMenuItem>Lorem ipsum</AsDropdownMenuItem>
        <AsDropdownMenuItem>Lorem ipsum</AsDropdownMenuItem>
      </AsInputDropdown>
    </AsInputGroup>
  </div>
  <div class="col-md-6 as-mb-24">
    <div class="as-mb-16">
      <label for="inputDir" class="as-text-16-semibold as-mb-8"
        >Email dan Domain</label
      >
      <AsInputGroup>
        <AsInput
          groupInput
          groupLeft
          type="text"
          id="inputDir"
          placeholder="no-reply"
        />
        <AsInputDropdown text="niagahoster.design">
          <AsDropdownMenuItem>Lorem ipsum</AsDropdownMenuItem>
          <AsDropdownMenuItem>Lorem ipsum</AsDropdownMenuItem>
          <AsDropdownMenuItem>Lorem ipsum</AsDropdownMenuItem>
        </AsInputDropdown>
      </AsInputGroup>
      <span id="idirectoryHelp" class="as-info as-info--secondary as-mb-8">
        Masukkan alamat email yang digunakan untuk menjawab secara otomatis.
        Anda hanya dapat membuat satu akun email autoresponder saja untuk
        masing-masing domain.
      </span>
    </div>
  </div>

  <div class="col-md-6 as-mb-24">
    <AsInputGroup>
      <AsInput
        groupInput
        groupLeft
        disabled
        type="text"
        id="inputDir"
        placeholder="no-reply"
      />
      <AsInputDropdown disabled text="niagahoster.design">
        <AsDropdownMenuItem>Lorem ipsum</AsDropdownMenuItem>
        <AsDropdownMenuItem>Lorem ipsum</AsDropdownMenuItem>
        <AsDropdownMenuItem>Lorem ipsum</AsDropdownMenuItem>
      </AsInputDropdown>
    </AsInputGroup>
  </div>
</template>

<script setup>
import AsInput from "./AsInput.vue";
import AsInputGroup from "./AsInputGroup.vue";
import AsInputDropdown from "./AsInputDropdown.vue";
import AsDropdownMenuItem from "../dropdown/AsDropdownMenuItem.vue";
</script>
