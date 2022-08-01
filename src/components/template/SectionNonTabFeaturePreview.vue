<template>
  <section class="as-section-soft">
    <div class="as-section__container">
      <h2 class="as-section__title as-text-32-bold as-lh-42 as-mb-20">
        Buat Website Impian Menjadi Nyata dengan Mudah
      </h2>
      <p class="as-section__description as-mb-32">
        Nikmati berbagai macam fitur dan manfaat yang mengesankan! Layanan web
        hosting Indonesia terbaik dan termurah dikelasnya.
      </p>

      <div class="as-section__flex as-gap-60 as-mb-32">
        <img
          src="~assets/images/samples/organism/feature-img-1.svg"
          alt="feature image 1"
          class="as-section__image w-100 as-mb-32"
        />
        <ul class="d-flex flex-column as-gap-40">
          <li>
            <h3 class="as-text-20-bold as-lh-26 as-mb-12">
              Miliki Website dengan Akses Tercepat
            </h3>
            <p class="as-text-16 as-lh-24 as-color-secondary-2">
              Percepat loading website dengan sederet fitur dan resource
              unggulan seperti:
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >SSD Disk Space</span
              >,
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >Data Center Tier 3</span
              >,
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >LiteSpeed Enterprise</span
              >, dan
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >WordPress Accelerator</span
              >, serta
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >jaminan uptime 99,9%</span
              >. Berikan kenyamanan lebih untuk pengunjung website Anda!
            </p>
          </li>
          <li>
            <h3 class="as-text-20-bold as-lh-26 as-mb-12">
              Tidak Harus Profesional Buat Kelola Website
            </h3>
            <p class="as-text-16 as-lh-24 as-color-secondary-2">
              Sekarang bisa dengan mudah kelola website tanpa harus mengerti
              dulu urusan teknis dan instalasi software! Dukungan
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >cPanel</span
              >
              dan
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >Softaculous</span
              >
              yang easy-to-use jadikan website siap online dalam beberapa menit.
            </p>
          </li>
          <li>
            <h3 class="as-text-20-bold as-lh-26 as-mb-12">
              Pantau Performa Website Hanya Sekali Klik
            </h3>
            <p class="as-text-16 as-lh-24 as-color-secondary-2">
              Hilangkan rasa khawatir saat website ada kendala dan buat kinerja
              website lebih cepat. Adanya fitur
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >PHP X-Ray</span
              >
              &
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >PageSpeed Insights</span
              >
              bantu memeriksa kondisi website. Pantau juga pengunjung website
              dengan fitur
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >Analytics Tools</span
              >.
            </p>
          </li>
        </ul>
      </div>

      <div class="as-section__flex as-gap-60 flex-row-reverse">
        <img
          src="~assets/images/samples/organism/feature-img-2.svg"
          alt="feature image 2"
          class="as-section__image w-100"
        />
        <ul class="d-flex flex-column as-gap-40">
          <li>
            <h3 class="as-text-20-bold as-lh-26 as-mb-12">
              24/7 Hosting Support
            </h3>
            <p class="as-text-16 as-lh-24 as-color-secondary-2">
              Sangat penting mendapatkan bantuan ketika dibutuhkan. Itu sebabnya
              dukungan Tim Profesional Niagahoster
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >24/7</span
              >
              selalu tersedia, termasuk masalah
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >Migrasi Website Gratis</span
              >.
            </p>
          </li>
          <li>
            <h3 class="as-text-20-bold as-lh-26 as-mb-12">
              Keamanan Website Jadi Perhatian Utama
            </h3>
            <p class="as-text-16 as-lh-24 as-color-secondary-2">
              Keamanan terjamin! Dilengkapi
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >Immunify360</span
              >,
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >Advanced Firewall</span
              >, dan
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >OS CloudLinux</span
              >
              kini tidak ada celah bagi hacker/cyber attack. Lindungi juga email
              Anda dari spam dengan fitur
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >SpamAssassin</span
              >
              dan
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >SpamExpert</span
              >.
            </p>
          </li>
          <li>
            <h3 class="as-text-20-bold as-lh-26 as-mb-12">
              Sarana Belajar Gratis! Raih Kesuksesan Online
            </h3>
            <p class="as-text-16 as-lh-24 as-color-secondary-2">
              Koleksi berbagai
              <span class="as-text-16-bold as-lh-24 as-color-secondary"
                >Course Premium</span
              >
              dari Niagahoster secara gratis dengan fasilitator expert. Lebih
              dari 10 bidang teknologi populer sebagai sarana untuk belajar dan
              raih kesuksesan online Anda lebih profesional.
            </p>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped>
@use "@/assets/scss/mixins/breakpoint" as *;

.as-section-soft {
  padding: 3.75rem 1.25rem 4rem;

  @include screen(tablet) {
    padding: 3.75rem 6rem 4rem;
  }

  @include screen(desktop) {
    padding: 7.5rem 8rem;
  }

  .as-section__title {
    @include screen(desktop) {
      text-align: center;
      font-size: 2.5rem;
      line-height: 3.5rem;
      letter-spacing: -0.02rem;
    }
  }

  .as-section__description {
    @include screen(desktop) {
      text-align: center;
      margin-bottom: 5rem;
    }
  }

  .as-section__image {
    max-width: 29.6875rem;

    @include screen(desktop) {
      margin-bottom: unset;
      min-width: 29.6875rem;
    }
  }

  .as-section__flex {
    @include screen(desktop) {
      margin-bottom: 5rem;
    }
  }
}
</style>
