<template>
  <ul class="as-nav-tabs">
    <li
      class="as-nav-tabs__item"
      v-for="(tab, index) in tabs"
      :key="index"
      :aria-setsize="tabs.length"
      :aria-posinet="index + 1"
    >
      <a
        href="javascript:void(0);"
        class="as-nav-tabs__link"
        :class="active_tab === index ? 'is-active' : ''"
        :aria-selected="active_tab === index"
        @click="changeTab(index)"
      >
        {{ tab.tab_title }}
      </a>
    </li>
  </ul>
  <div class="as-nav-content">
    <div
      v-for="(tab, index) in tabs"
      :key="index"
      :aria-current="active_tab === index"
      class="as-nav-pane"
      v-show="active_tab === index"
    >
      <p>{{ tab.tab_content }}</p>
    </div>
  </div>
</template>

<style lang="scss">
@use "@/assets/scss/components/tab.scss";
</style>

<script setup>
const active_tab = ref(0);
const tabs = [
  {
    tab_title: "Mobile Banking",
    tab_content:
      "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Beatae quae eligendi illum impedit distinctio, quasi ex minus omnis, in sunt, quos corrupti dolore et laboriosam doloribus dignissimos nostrum cumque repellendus.",
  },
  {
    tab_title: "ATM",
    tab_content:
      "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora libero quos quibusdam adipisci nesciunt ducimus? Necessitatibus libero debitis dolorem delectus.",
  },
  {
    tab_title: "Internet Banking",
    tab_content:
      "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Blanditiis dolorem quis distinctio, deleniti consequuntur labore numquam repudiandae cumque repellendus libero praesentium ipsum fuga earum eius.",
  },
];

function changeTab(tabIndexValue) {
  active_tab.value = tabIndexValue;
}
</script>
