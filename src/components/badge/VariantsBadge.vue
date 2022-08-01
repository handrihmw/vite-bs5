<template>
  <AsTable striped>
    <thead class="as-mb-24">
      <tr class="as-color-primary">
        <th scope="col" class="as-text-16-bold">Variant</th>
        <th scope="col" class="as-text-16-bold">Usage</th>
      </tr>
    </thead>
    <tbody class="as-table__striped">
      <AsTableRow v-for="item in items" :key="item.id">
        <td scope="row">
          <p class="as-text-16-semibold">
            {{ item.name }}
          </p>
        </td>
        <td>
          <ul class="d-flex flex-column gap-1">
            <li v-for="use in item.usage" :key="use.id">
              <p class="as-text-16">
                Use
                <code>{{ use.code }}</code> classes
              </p>
            </li>
          </ul>
        </td>
      </AsTableRow>
    </tbody>
  </AsTable>
</template>

<script setup>
import AsTable from "../../components/table/AsTable.vue";
import AsTableRow from "../../components/table/AsTableRow.vue";

import badgeVariantData from "~/store/variants/badgeVariant.json";
const items = badgeVariantData;
</script>

<style lang="scss" scoped>
@use "@/assets/scss/mixins/breakpoint" as *;
ul {
  margin: 0;
  padding: 0;
  li {
    list-style-type: none;
    padding: 0;
  }
}
</style>
