<template>
  <section class="as-section as-section-soft">
    <div class="as-section__container">
      <div class="row gy-4 gy-lg-5">
        <div
          class="as-bonus-item col-lg-4"
          v-for="item in dataBonus"
          :key="item.id"
        >
          <div>
            <div class="as-bonus-item__ribbon">
              <span class="as-ribbon as-ribbon--green">GRATIS</span>
            </div>

            <h3 class="as-bonus-item__title">{{ item.title }}</h3>
          </div>

          <p class="as-bonus-item__description">
            {{ item.description }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const dataBonus = [
  {
    title: "Domain senilai Rp. 175.000",
    description:
      "Gratis domain ekstensi com, .net, .org, or.id, ac.id, .website, .info dan banyak lagi!",
  },
  {
    title: "Perlindungan SSL Let’s Encrypt",
    description:
      "Jadikan website Anda lebih aman dan terpercaya dengan perlindungan SSL",
  },
  {
    title: "Akun Email Profesional",
    description:
      "Buat akun email professional dengan nama domain Anda. Jadikan bisnis lebih terpercaya",
  },
  {
    title: "Bantuan Migrasi Web Hosting",
    description:
      "Dapatkan bantuan migrasi file website ke web hosting Niagahoster secara gratis.",
  },
  {
    title: "Layanan Backup Mingguan hingga Harian",
    description:
      "Jangan khawatir data website hilang, fitur backup otomatis menjamin data tetap aman",
  },
  {
    title: "Course Premium dengan Mentor Para Expert",
    description:
      "Kesempatan belajar langsung bersama para expert untuk gapai kesuksesan online",
  },
];
</script>

<style lang="scss">
@use "@/assets/scss/mixins/breakpoint" as *;

.as-bonus-item {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 0.75rem;

  &__ribbon {
    margin-bottom: 1.5rem;
    display: flex;
  }
  &__title {
    font-family: NunitoSansRegular, sans-serif;
    font-weight: 700;
    font-size: 1.25rem;
    line-height: 1.625em;
    color: var(--as-color-primary);
  }
  &__description {
    font-family: NunitoSansRegular, sans-serif;
    font-size: 1rem;
    line-height: 1.5em;
    letter-spacing: 0.005rem;
    color: var(--as-color-secondary);
  }
}
</style>
