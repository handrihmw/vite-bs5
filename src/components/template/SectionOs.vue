<template>
  <section class="as-section-soft as-py-60 as-px-20">
    <div class="as-section__container">
      <h2 class="as-section__title as-mb-32 as-max-width-920 as-mx-auto">
        Pilih Sistem Operasi dan Panel untuk Kebutuhan VPS Hosting Anda
      </h2>
      <p class="as-section__description as-mb-32 as-max-width-920 as-mx-auto">
        Kustomisasi sistem operasi & panel Anda melalui satu dasbor saja. Pilih
        OS untuk VPS Anda dari CentOS hingga Suse, dengan atau tanpa panel hanya
        di Niagahoster.
      </p>

      <ul class="as-section-os--mobile">
        <li v-for="item in dataOs" :key="item.id">
          <img :src="item.illustration" :alt="item.alt" class="w-75 as-mb-32" />

          <h3 class="as-section__title as-mb-32">{{ item.title }}</h3>
          <p class="as-section__description as-mb-42">
            {{ item.description }}
          </p>

          <ul class="os-list-mobile as-list-icon as-pl-28">
            <li
              class="as-list-icon__item as-list-icon__item--xlg as-list-icon__item--with-tooltip"
              v-for="list in item.osList"
              :key="list.id"
              :class="[expandable ? 'os-list-mobile--show' : 'hide']"
            >
              <span>{{ list.os }}</span>

              <div class="as-tooltip" v-if="list.tooltip">
                <img
                  src="~assets/images/samples/tooltip-icon.svg"
                  alt="tooltip icon"
                  class="as-width-28"
                />
                <p
                  class="as-tooltip__info as-tooltip__info--top as-text-14 as-lh-24"
                >
                  {{ list.tooltipText }}
                </p>
              </div>
            </li>
          </ul>

          <button
            class="as-btn--fluid as-link as-link-icon as-link--transparent"
            @click="showList"
          >
            <div v-if="!expandable" class="as-text-16-bold">
              <span>Lihat Sebagian</span>
              <i class="as-icon-arrow-top as-ml-24 as-width-10"></i>
            </div>

            <div v-else class="as-text-16-bold">
              <span>Lihat Semua</span>
              <i class="as-icon-arrow-down as-ml-24"></i>
            </div>
          </button>
        </li>
      </ul>

      <ul class="as-section-os--desktop">
        <li
          v-for="item in dataOs"
          :key="item.id"
          class="d-flex flex-row-reverse justify-content-between as-gap-42"
        >
          <div class="as-section__image as-width-420 as-min-width-300">
            <img :src="item.illustration" :alt="item.alt" />
          </div>

          <div class="as-max-width-635">
            <h3 class="as-section__title as-mb-32">{{ item.title }}</h3>
            <p class="as-section__description as-mb-42">
              {{ item.description }}
            </p>

            <ul class="os-list-desktop as-list-icon as-pl-28">
              <li
                class="as-list-icon__item as-list-icon__item--xlg as-list-icon__item--with-tooltip"
                v-for="list in item.osList"
                :key="list.id"
              >
                <span>{{ list.os }}</span>

                <div class="as-tooltip" v-if="list.tooltip">
                  <img
                    src="~assets/images/samples/tooltip-icon.svg"
                    alt="tooltip icon"
                    class="as-width-28"
                  />
                  <p
                    class="as-tooltip__info as-tooltip__info--top as-text-14 as-lh-24"
                  >
                    {{ list.tooltipText }}
                  </p>
                </div>
              </li>
            </ul>
          </div>
        </li>
      </ul>
    </div>
  </section>

  <section class="as-section-blue as-py-32 as-px-20">
    <div class="as-section__container">
      <div class="as-section__flex as-gap-120">
        <div class="as-section__image as-mb-32 as-mx-20">
          <img
            src="~assets/images/samples/organism/cloudvpshosting/illust-os-2.svg"
            alt="Illustration OS"
            loading="lazy"
          />
        </div>

        <div>
          <h2 class="as-section__title as-mb-32">
            Ganti OS Dengan Mudah di Cloud VPS Niagahoster
          </h2>
          <p class="as-section__description as-mb-32">
            Nikmati beragam OS dengan teknologi dan fitur terbaik dari VPS murah
            terbaik di Indonesia. Kelola website dan segala kebutuhan online
            Anda tanpa repot di Niagahoster!
          </p>
          <button class="as-btn as-btn--primary as-btn--fluid">
            Pesan Sekarang
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import imgCent from "@/assets/images/samples/organism/cloudvpshosting/cent.svg";

const dataOs = [
  {
    illustration: imgCent,
    alt: "Cent OS Illustration",
    title: "CentOS",
    description:
      "Terinspirasi dari Red Hat Enterprise Linux, CentOS adalah salah satu sistem operasi enterprise terunggul, dan pilihan terbaik untuk VPS Anda dengan kecepatan ekstra, stabilitas yang handal, serta keamanan yang terjamin.",

    osList: [
      {
        os: "CentOS 6 64bit",
        tooltip: false,
        tooltipText: "",
      },
      {
        os: "CentOS 7 64bit",
        tooltip: false,
        tooltipText: "",
      },
      {
        os: "CentOS 7 64bit minimal",
        tooltip: false,
        tooltipText: "",
      },

      {
        os: "CentOS 7 64bit with CentOS Panel",
        tooltip: false,
        tooltipText: "",
      },
      {
        os: "CentOS 7 64bit with CyberPanel",
        tooltip: false,
        tooltipText: "",
      },
      {
        os: "CentOS 7 64bit with Plesk Onyx",
        tooltip: false,
        tooltipText: "",
      },
      {
        os: "CentOS 7 64bit with Webmin",
        tooltip: false,
        tooltipText: "",
      },
      {
        os: "CentOS 7 64bit with Webmin/Virtualmin/LAMP",
        tooltip: false,
        tooltipText: "",
      },
      {
        os: "CentOS 7 64bit with Webuzo control panel",
        tooltip: true,
        tooltipText:
          "Dapatkan beragam fitur premium dengan lisensi Webuzo. Lihat informasi terkait pembelian Lisensi Webuzo di sini. ",
      },
      {
        os: "CentOS 7 64bit with Plesk Onyx",
        tooltip: false,
        tooltipText: "",
      },
      {
        os: "CentOS 7 64bit with cPanel and WHM",
        tooltip: true,
        tooltipText:
          "Khusus untuk lisensi cPanel dan WHM dibeli secara terpisah. Lihat informasi terkait pembelian Lisensi cPanel di sini.",
      },
    ],
  },
];

const expandable = ref(true);

const showList = () => {
  expandable.value = !expandable.value;
};
</script>

<style lang="scss">
@use "@/assets/scss/mixins/breakpoint" as *;
li {
  list-style-type: none;
}

.as-section-soft {
  @include screen(desktop) {
    padding-block: 7.5rem;
  }

  .as-section__title,
  .as-section__description {
    @include screen(desktop) {
      text-align: center;
    }
  }

  .as-section-os--desktop {
    .as-section__title,
    .as-section__description {
      text-align: left;
    }
  }
}
</style>
