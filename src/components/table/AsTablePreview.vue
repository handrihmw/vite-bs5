<template>
  <AsTable striped>
    <thead class="as-mb-24">
      <tr class="as-color-primary">
        <th scope="col" class="as-text-16-bold">Produk & Layanan</th>
        <th scope="col" class="as-text-16-bold">Aktif hingga</th>
        <th scope="col" class="as-text-16-bold">Status</th>
        <th scope="col"></th>
      </tr>
    </thead>
    <tbody>
      <AsTableRow v-for="item in items" :key="item.id">
        <th scope="row">
          <div class="d-flex gap-3 align-items-center">
            <img
              :src="item.product.image"
              class="img-fluid"
              loading="lazy"
              alt="thumb"
            />
            <div>
              <p class="as-text-20-bold as-color-primary">
                {{ item.product.domain }}
              </p>
              <p class="as-text-12 as-color-secondary-2">
                {{ item.product.type }}
              </p>
            </div>
          </div>
        </th>
        <td>
          <p class="as-text-16-semibold as-color-primary">
            {{ item.period.date_end }}
          </p>
          <p class="as-text-12 as-color-secondary-2">
            {{ item.period.year }}
          </p>
        </td>
        <td>
          <AsBadge :class="`as-badge--${item.status.label}`">{{
            item.status.info
          }}</AsBadge>
        </td>
        <td class="text-end">
          <AsButton anchor href="#" primary sm>Kelola Hosting</AsButton>
        </td>
      </AsTableRow>
    </tbody>
  </AsTable>
</template>

<script setup>
import AsTable from "./AsTable.vue";
import AsTableRow from "./AsTableRow.vue";
import AsBadge from "../badge/AsBadge.vue";
import AsButton from "../button/AsButton.vue";

import dtTables1 from "~/store/data/table1.json";
const items = dtTables1;
</script>
