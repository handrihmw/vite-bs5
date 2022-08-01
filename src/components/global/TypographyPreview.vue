<template>
  <AsTable striped>
    <thead class="as-mb-24">
      <tr class="as-color-primary">
        <th scope="col" class="as-text-16-bold">Scale Category</th>
        <th scope="col" class="as-text-16-bold">Typeface</th>
        <th scope="col" class="as-text-16-bold">Weight</th>
        <th scope="col" class="as-text-16-bold">Size / Line Height</th>
        <th scope="col" class="as-text-16-bold">Case</th>
        <th scope="col" class="as-text-16-bold">letter Spacing</th>
      </tr>
    </thead>
    <tbody class="as-table__striped">
      <AsTableRow v-for="item in items" :key="item.id">
        <td scope="row">
          <p :class="item.class">{{ item.scale }}</p>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">
            {{ item.typeface }}
          </p>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">{{ item.weight }}</p>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">
            {{ item.sizeLineHeight }}
          </p>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">{{ item.case }}</p>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">
            {{ item.letterSpacing }}
          </p>
        </td>
      </AsTableRow>
    </tbody>
  </AsTable>
</template>

<script setup>
import AsTable from "../table/AsTable.vue";
import AsTableRow from "../table/AsTableRow.vue";

import typographyData from "~/store/data/typography.json";
const items = typographyData;
</script>

<style lang="scss" scoped></style>
