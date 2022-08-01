<template>
  <section class="as-section-white as-mb-60">
    <div class="as-section__container">
      <table
        class="as-table-border as-table-border--fluid as-mb-40"
        id="domain-prices-table"
      >
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

      <table
        class="as-table-border as-table-border--fluid as-table-border--domain"
        id="domain-prices-table"
      >
        <tbody>
          <tr v-for="item in dataDomain" :key="item.id">
            <td class="as-table-border__name">{{ item.domain }}</td>
            <td class="as-table-border__price">
              <div
                class="d-flex align-items-center as-gap-24 as-mb-8"
                v-if="item.isDiscount"
              >
                <span class="as-ribbon as-ribbon--red"
                  >Diskon {{ item.discount }}</span
                >
                <del class="as-text-14-bold as-lh-16 as-color-secondary">{{
                  item.priceBefore
                }}</del>
              </div>
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
    </div>
  </section>
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

<style lang="scss"></style>
