<template>
  <section class="as-section-soft">
    <div class="as-section__container">
      <h2
        class="as-text-32-bold as-lh-42 as-color-primary as-mb-24 text-center"
      >
        Solusi Untuk Beragam Kebutuhan Anda
      </h2>
      <p class="as-section__description as-mb-36 text-center">
        Penawaran VPS KVM kini semakin optimal, mendukung segala kebutuhan
        website online Anda.
      </p>

      <ul class="feature-card-container as-mb-36">
        <li
          class="as-feature-card as-card as-card__container--xlg as-border-radius-24"
          v-for="item in dataOffer"
          :key="item.id"
        >
          <img :src="item.icon" :alt="item.alt" class="as-width-66 as-mb-24" />
          <h3 class="as-text-20-bold as-lh-26 as-color-primary as-mb-14">
            {{ item.title }}
          </h3>
          <p class="as-text-16 as-lh-24 as-color-secondary-2 as-mb-26">
            {{ item.description }}
          </p>

          <ul class="as-list-icon as-pl-28">
            <li
              class="as-list-icon__item as-list-icon__item--sm as-list-icon__item--sm-blue as-list-icon__item--with-tooltip"
              v-for="list in item.offerList"
              :key="list.id"
            >
              <span>{{ list }}</span>

              <div class="as-tooltip">
                <img
                  src="~assets/images/samples/tooltip-icon.svg"
                  alt="tooltip icon"
                  class="as-width-16"
                />
                <p
                  class="as-tooltip__info as-tooltip__info--top as-text-14 as-lh-24"
                >
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa,
                  officia praesentium laudantium in fugiat excepturi.
                </p>
              </div>
            </li>
          </ul>
        </li>
      </ul>

      <p
        class="as-text-16 as-lh-24 as-color-secondary text-center as-mb-28 as-mx-auto as-width-540"
      >
        Dapatkan penawaran menarik untuk segala kebutuhan online Anda hanya di
        Niagahoster
      </p>
      <button class="as-btn as-btn--primary as-btn--fluid as-mx-auto">
        Lihat Penawaran
      </button>
    </div>
  </section>
</template>

<script setup>
import imgEdu from "@/assets/images/samples/organism/vpskvm/offer-education.svg";
import imgBus from "@/assets/images/samples/organism/vpskvm/offer-business.svg";
import imgNew from "@/assets/images/samples/organism/vpskvm/offer-news.svg";
import imgOrg from "@/assets/images/samples/organism/vpskvm/offer-organization.svg";
import imgDev from "@/assets/images/samples/organism/vpskvm/offer-development.svg";
import imgFrx from "@/assets/images/samples/organism/vpskvm/offer-forex.svg";

const dataOffer = [
  {
    icon: imgEdu,
    alt: "Icon Offer Education",
    title: "E-Learning & Education",
    description:
      "Kelola urusan akademik, dengan penyimpanan data yang lebih besar",
    offerList: [
      "Server Ujian Online",
      "Sistem Akademik",
      "Learning Management",
      "Website Sekolah",
      "Website Universitas",
    ],
  },
  {
    icon: imgBus,
    alt: "Icon Offer Business",
    title: "Bisnis & Produktivitas",
    description:
      "Optimalkan performa website untuk kebutuhan bisnis & produktivitas Anda",
    offerList: [
      "E-commerce/Toko Online",
      "Enterprise Resource Planning (ERP)",
      "CRM Application Development",
      "Sistem Informasi Akutansi",
      "Internet of Things (IoT)",
    ],
  },
  {
    icon: imgNew,
    alt: "Icon Offer News",
    title: "Portal Berita",
    description:
      "Tingkatkan performa portal berita online Anda dengan beragam fitur",
    offerList: [
      "Portal Berita Online",
      "Video Streaming Websites",
      "Online Event",
      "Online Magazine",
      "Website Review",
    ],
  },
  {
    icon: imgOrg,
    alt: "Icon Offer Organization",
    title: "Instansi & Organisasi",
    description:
      "Penyimpanan yang lebih besar untuk mengelola instansi & organisasi Anda",
    offerList: [
      "Website Pemerintahan",
      "Sistem Kepegawaian",
      "E-Budgeting",
      "Crowdfunding",
      "Komunitas Online",
    ],
  },
  {
    icon: imgDev,
    alt: "Icon Offer Development",
    title: "Development & Test Server",
    description: "Fitur terlengkap untuk keperluan testing development Anda.",
    offerList: [
      "Docker",
      "MS SQL Server",
      "Online Storage",
      "File Sharing Platform",
      "Mobile Application Server",
    ],
  },
  {
    icon: imgFrx,
    alt: "Icon Offer Forex",
    title: "Forex Trader VPS",
    description: "Buat dan kelola sistem trading terbaik sesuai kebutuhan Anda",
    offerList: ["Meta Trader 4", "RDP", "Windows Server Application"],
  },
];
</script>

<style lang="scss">
@use "@/assets/scss/mixins/breakpoint" as *;

.as-section-soft {
  padding: 2.25rem 1.25rem;
  overflow: hidden;

  @include screen(desktop) {
    padding-block: 3.625rem;
  }

  .as-section__description {
    @include screen(desktop) {
      margin-bottom: 3rem;
    }
  }

  .feature-card-container {
    list-style-type: none;
    display: flex;
    flex-direction: column;
    gap: 2.25rem;

    @include screen(desktop) {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(21.875rem, 1fr));
      gap: 1.875rem;
      margin-bottom: 3rem;
    }
  }

  .as-btn {
    @include screen(desktop) {
      width: fit-content;
      padding-inline: 4.875rem;
    }
  }
}
</style>
