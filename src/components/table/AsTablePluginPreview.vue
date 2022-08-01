<template>
  <AsTable striped>
    <thead class="as-mb-24">
      <tr class="as-color-primary">
        <th scope="col" class="as-text-16-bold">Plugin</th>
        <th scope="col" class="as-text-16-bold">Versi</th>
        <th scope="col"></th>
      </tr>
    </thead>
    <tbody>
      <AsTableRow v-for="item in items" :key="item.id">
        <th scope="row">
          <div class="d-flex gap-3 align-items-center">
            <img
              :src="item.image"
              class="img-fluid"
              loading="lazy"
              alt="thumb"
            />
            <div>
              <p class="as-text-20-bold as-color-primary">
                {{ item.name }}
              </p>
              <p class="as-text-12 as-color-secondary-2">
                {{ item.description }}
              </p>
            </div>
          </div>
        </th>
        <td>
          <p class="as-text-16-semibold as-color-primary">
            {{ item.version }}
          </p>
        </td>
        <td>
          <AsSwitcher :id="'switch-' + item.id"> </AsSwitcher>
        </td>
      </AsTableRow>
    </tbody>
  </AsTable>
</template>

<script setup>
import AsTable from "./AsTable.vue";
import AsTableRow from "./AsTableRow.vue";
import AsSwitcher from "../switcher/AsSwitcher.vue";

import dtTables3 from "~/store/data/table3.json";
const items = dtTables3;
</script>
