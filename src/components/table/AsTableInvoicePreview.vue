<template>
  <AsTable striped>
    <thead class="as-mb-24">
      <tr class="as-color-primary">
        <th scope="col" class="as-text-16-bold">Nomor Tagihan</th>
        <th scope="col" class="as-text-16-bold">Nominal Tagihan</th>
        <th scope="col" class="as-text-16-bold">Pesanan Dibuat</th>
        <th scope="col" class="as-text-16-bold">Tanggal Jatuh Tempo</th>
        <th scope="col"></th>
      </tr>
    </thead>
    <tbody>
      <AsTableRow v-for="item in items" :key="item.id">
        <th scope="row">
          <div class="d-flex align-items-center gap-3 as-mb-8">
            <p class="as-text-20-bold as-color-primary">
              #{{ item.invoice.id }}
            </p>
            <AsBadge :class="`as-badge--${item.invoice.status.label}`">{{
              item.invoice.status.info
            }}</AsBadge>
          </div>
          <ul
            v-for="order_item in item.invoice.order"
            :key="item.invoice.order"
          >
            <li class="as-text-12 as-color-secondary-2 as-mb-4">
              {{ order_item }}
            </li>
          </ul>
        </th>
        <td>
          <p class="as-text-16-semibold as-color-primary as-mb-4">
            {{ item.nominal.amount }}
          </p>
          <p class="as-text-12 as-color-secondary-2">
            {{ item.nominal.bank }}
          </p>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-primary">
            {{ item.order_date }}
          </p>
        </td>
        <td>
          <p class="as-text-16-semibold as-color-red">
            {{ item.due_date }}
          </p>
        </td>
        <td>
          <AsButtonIcon disabled sm class="as-border-radius-8">
            <i class="as-icon-dot"></i>
          </AsButtonIcon>
        </td>
      </AsTableRow>
    </tbody>
  </AsTable>
</template>

<script setup>
import AsTable from "./AsTable.vue";
import AsTableRow from "./AsTableRow.vue";
import AsBadge from "../badge/AsBadge.vue";
import AsButtonIcon from "../button/AsButtonIcon.vue";

import dtTables2 from "~/store/data/table2.json";
const items = dtTables2;
</script>
