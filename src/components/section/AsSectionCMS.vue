<template>
  <section class="as-section as-py-64">
    <div
      class="as-section__container d-lg-flex align-items-lg-center justify-content-lg-between gap-lg-5"
    >
      <h2 class="as-text-28-bold as-lh-36 as-mb-40 mb-lg-0 as-max-width-320">
        Telah dioptimasi untuk berbagai CMS dan framework
      </h2>
      <div class="d-block d-lg-none">
        <ul class="row">
          <li class="col-4 text-center" v-for="item in dataCms" :key="item.id">
            <img
              :src="item.img"
              :alt="item.alt"
              loading="lazy"
              width="82"
              height="40"
              class="blur-up lazyloaded"
            />
          </li>
        </ul>
      </div>

      <div class="d-none d-lg-block">
        <ul class="row as-max-width-730 as-px-60">
          <li
            class="col-4 as-px-8 text-center"
            v-for="item in dataCms"
            :key="item.id"
          >
            <img
              :src="item.imgDesktop"
              :alt="item.alt"
              loading="lazy"
              width="162"
              height="56"
              class="blur-up lazyloaded"
            />
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script setup>
import imgWPMobile from "@/assets/images/hosting-indonesia/wordpress-mobile.webp";
import imgJoomlaMobile from "@/assets/images/hosting-indonesia/joomla-mobile.webp";
import imgPSMobile from "@/assets/images/hosting-indonesia/prestashop-mobile.webp";
import imgLaravelMobile from "@/assets/images/hosting-indonesia/laravel-mobile.webp";
import imgNodeMobile from "@/assets/images/hosting-indonesia/nodejs-mobile.webp";
import imgPyMobile from "@/assets/images/hosting-indonesia/python-mobile.webp";

import imgWP from "@/assets/images/hosting-indonesia/wordpress.webp";
import imgJoomla from "@/assets/images/hosting-indonesia/joomla.webp";
import imgPS from "@/assets/images/hosting-indonesia/prestashop.webp";
import imgLaravel from "@/assets/images/hosting-indonesia/laravel.webp";
import imgDrupal from "@/assets/images/hosting-indonesia/drupal.webp";
import imgOC from "@/assets/images/hosting-indonesia/opencart.webp";
const dataCms = [
  {
    img: imgWPMobile,
    imgDesktop: imgWP,
    alt: "WordPress",
  },
  {
    img: imgJoomlaMobile,
    imgDesktop: imgJoomla,
    alt: "Joomla",
  },
  {
    img: imgPSMobile,
    imgDesktop: imgPS,
    alt: "PrestaShop",
  },
  {
    img: imgLaravelMobile,
    imgDesktop: imgLaravel,
    alt: "Laravel",
  },
  {
    img: imgNodeMobile,
    imgDesktop: imgDrupal,
    alt: "Drupal",
  },
  {
    img: imgPyMobile,
    imgDesktop: imgOC,
    alt: "Opencart",
  },
];
</script>
