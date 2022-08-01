<template>
  <AsTable striped>
    <thead class="as-mb-24">
      <tr class="as-color-primary">
        <th scope="col" class="as-text-16-bold">Breakpoints</th>
        <th scope="col" class="as-text-16-bold">Helper</th>
        <th scope="col" class="as-text-16-bold">Dimensions</th>
      </tr>
    </thead>
    <tbody class="as-table__striped">
      <AsTableRow>
        <td scope="row">
          <p class="as-text-16-semibold as-color-primary">Mobile Small</p>
        </td>
        <td>
          <code> @include screen(mobileSmall) </code>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">&lt; 576px</p>
        </td>
      </AsTableRow>
      <AsTableRow>
        <td scope="row">
          <p class="as-text-16-semibold as-color-primary">Mobile</p>
        </td>
        <td>
          <code> @include screen(mobile) </code>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">&ge; 576px</p>
        </td>
      </AsTableRow>
      <AsTableRow>
        <td scope="row">
          <p class="as-text-16-semibold as-color-primary">Tablet</p>
        </td>
        <td>
          <code> @include screen(tablet) </code>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">&ge; 768px</p>
        </td>
      </AsTableRow>
      <AsTableRow>
        <td scope="row">
          <p class="as-text-16-semibold as-color-primary">Desktop</p>
        </td>
        <td>
          <code> @include screen(desktop) </code>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">&ge; 992px</p>
        </td>
      </AsTableRow>
      <AsTableRow>
        <td scope="row">
          <p class="as-text-16-semibold as-color-primary">Desktop Big</p>
        </td>
        <td>
          <code> @include screen(desktopBig) </code>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">&ge; 1200px</p>
        </td>
      </AsTableRow>
      <AsTableRow>
        <td scope="row">
          <p class="as-text-16-semibold as-color-primary">Desktop Large</p>
        </td>
        <td>
          <code> @include screen(desktopLarge) </code>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">&ge; 1400px</p>
        </td>
      </AsTableRow>
      <AsTableRow>
        <td scope="row">
          <p class="as-text-16-semibold as-color-primary">Desktop Extra</p>
        </td>
        <td>
          <code> @include screen(desktopExtra) </code>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">&ge; 1920px</p>
        </td>
      </AsTableRow>
    </tbody>
  </AsTable>
</template>

<script setup>
import AsTable from "../../components/table/AsTable.vue";
import AsTableRow from "../../components/table/AsTableRow.vue";
</script>

<style lang="scss" scoped></style>
