<template>
  <table class="as-table-border w-75 as-mb-40" id="domain-prices-table">
    <tbody>
      <tr v-for="item in dataDomain" :key="item.id">
        <td class="as-table-border__name">{{ item.domain }}</td>
        <td class="as-table-border__price">
          <p>
            {{ item.priceFinal }}
          </p>
        </td>
        <td class="as-table-border__action">
          <button class="as-btn as-btn--primary as-btn--fluid as-btn--sm">
            Beli
          </button>
        </td>
      </tr>
    </tbody>
  </table>
</template>

<script setup>
const dataDomain = [
  {
    domain: ".com",
    isDiscount: true,
    discount: "25%",
    priceBefore: "Rp. 200.000,-",
    priceFinal: "Rp. 125.000,-",
  },
  {
    domain: ".id",
    isDiscount: true,
    discount: "25%",
    priceBefore: "Rp. 200.000,-",
    priceFinal: "Rp. 125.000,-",
  },
  {
    domain: ".co.id",
    isDiscount: false,
    discount: "",
    priceBefore: "",
    priceFinal: "Rp. 125.000,-",
  },
];
</script>

<style lang="scss">
@use "../../assets/scss/components/table";
</style>
