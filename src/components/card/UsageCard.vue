<template>
  <AsTable striped>
    <thead class="as-mb-24">
      <tr class="as-color-primary">
        <th scope="col" class="as-text-16-bold">Class</th>
        <th scope="col" class="as-text-16-bold">Props</th>
        <th scope="col" class="as-text-16-bold">Types</th>
        <th scope="col" class="as-text-16-bold">Description</th>
      </tr>
    </thead>
    <tbody class="as-table__striped">
      <AsTableRow v-for="item in items" :key="item.id">
        <td scope="row">
          <p>
            <code>{{ item.class }}</code>
          </p>
        </td>
        <td>
          <ul class="d-flex flex-column gap-1">
            <li v-for="prop in item.props" :key="prop.id">
              <p>
                <code>{{ prop.name }}</code>
              </p>
            </li>
          </ul>
        </td>
        <td>
          <ul class="d-flex flex-column gap-1">
            <li v-for="prop in item.props" :key="prop.id">
              <p>
                <code>{{ prop.types }}</code>
              </p>
            </li>
          </ul>
        </td>
        <td>
          <ul class="d-flex flex-column gap-1">
            <li v-for="prop in item.props" :key="prop.id">
              <p>{{ prop.description }}</p>
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

import cardData from "~/store/usage/card.json";
const items = cardData;
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
