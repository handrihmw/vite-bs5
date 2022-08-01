<template>
  <section class="as-section-white as-py-40">
    <div class="as-section__container">
      <div
        class="as-section__flex as-gap-48 as-pb-40 as-border-bottom as-mb-24 as-mx-20"
      >
        <img
          src="~assets/images/samples/organism/vpskvm/illust-performance.svg"
          alt="Illustration Benchmark Performance"
          class="as-section__image w-100"
          loading="lazy"
        />
        <div class="performance-text as-mt-40">
          <p
            class="performance-text__identifier as-mb-18 as-text-18-bold as-lh-27 as-color-secondary"
          >
            Raih Performa Prima dengan Cloud VPS KVM dan ESSD!
          </p>
          <h2 class="as-section__title as-mb-24">
            Performa Hebat dengan Virtualisasi Berbasis Kernel
          </h2>
          <p class="as-section__description">
            Teknologi termutakhir dan sumber daya terdedikasi dari Cloud VPS KVM
            Niagahoster bantu meningkatkan kecepatan infrastruktur hosting Anda.
            Performa website tetap handal, meski saat traffic tinggi!
          </p>
        </div>
      </div>

      <ul class="as-slider-simple as-px-20 as-py-16 as-mb-24">
        <li
          class="as-benchmark-card as-card as-card__container--benchmark as-card__section justify-content-between as-border-radius-12 as-mb-0"
          v-for="item in dataPerformance"
          :key="item.id"
        >
          <h3 class="as-text-16-semibold as-lh-24 as-color-green">
            {{ item.title }}
          </h3>
          <div>
            <p class="as-text-56 as-lh-64">
              {{ item.value
              }}<span class="as-text-24-bold as-lh-32 as-ml-4">{{
                item.unit
              }}</span>
            </p>
            <p class="as-text-16 as-lh-24 as-color-secondary-2">Up to</p>
          </div>
        </li>
      </ul>

      <p class="as-mx-20 as-text-16 as-lh-24 as-color-secondary text-center">
        *Pengujian dilakukan dengan paketVPS Super Power
      </p>
    </div>
  </section>
</template>

<script setup>
const dataPerformance = [
  {
    title: "Bandwidth Speed",
    value: "30",
    unit: "Mbps",
  },
  {
    title: "Geekbench Single-Core (CPU)",
    value: "862",
    unit: "Point",
  },
  {
    title: "Geekbench Multi-Core (CPU)",
    value: "2647",
    unit: "Point",
  },
  {
    title: "Network Speed (Download)",
    value: "100",
    unit: "MB/s",
  },
  {
    title: "Network Speed (Upload)",
    value: "30",
    unit: "MB/s",
  },
  {
    title: "Disk Speed - I/O ",
    value: "230",
    unit: "MB/s",
  },
];
</script>

<style lang="scss">
@use "@/assets/scss/mixins/breakpoint" as *;
.as-section-white {
  @include screen(desktop) {
    padding-block: 7.5rem;
  }

  .as-section__flex {
    .as-section__image {
      @include screen(desktop) {
        max-width: 29.6875rem;
      }
    }

    .performance-text {
      &__identifier {
        @include screen(desktop) {
          margin-bottom: 1.5rem;
        }
      }

      .as-section__title {
        @include screen(desktop) {
          margin-bottom: 2rem;
        }
      }

      @include screen(desktop) {
        margin-top: unset;
      }
    }

    @include screen(desktop) {
      display: flex;
      align-items: center;
      gap: 3rem;
      padding-bottom: 0.5rem;
    }
  }

  .as-slider-simple {
    @include screen(desktop) {
      gap: 0.875rem;
      row-gap: 2.5rem;
    }
  }
}
</style>
