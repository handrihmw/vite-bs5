<template>
  <AsTabLine>
    <li
      class="as-nav-line__item"
      v-for="(tab, index) in tabs"
      :key="index"
      :aria-setsize="tabs.length"
      :aria-posinet="index + 1"
    >
      <a
        href="javascript:void(0);"
        class="as-nav-line__link as-btn-icon"
        :class="active_tab === index ? 'is-active' : ''"
        :aria-selected="active_tab === index"
        @click="changeTabLine(index)"
      >
        {{ tab.tab_title }}
      </a>
    </li>
  </AsTabLine>
  <AsTabLineContent>
    <div
      v-for="(tab, index) in tabs"
      :key="index"
      :aria-current="active_tab === index"
      class="as-nav-pane"
      v-show="active_tab === index"
    >
      <p>{{ tab.tab_content }}</p>
    </div>
  </AsTabLineContent>
</template>

<script setup>
import AsTabLine from "./AsTabLine.vue";
import AsTabLineItem from "./AsTabLineItem.vue";
import AsTabLineContent from "./AsTabLineContent.vue";

const active_tab = ref(0);
const tabs = [
  {
    tab_title: "Plugin Terinstall",
    tab_content:
      "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Beatae quae eligendi illum impedit distinctio, quasi ex minus omnis, in sunt, quos corrupti dolore et laboriosam doloribus dignissimos nostrum cumque repellendus. Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo ex obcaecati accusantium temporibus minus accusamus odio magnam, maiores voluptas sapiente, qui aliquam porro doloribus? Adipisci placeat suscipit consectetur possimus dolore?",
  },
  {
    tab_title: "Tambah Plugin Baru",
    tab_content:
      "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora libero quos quibusdam adipisci nesciunt ducimus? Necessitatibus libero debitis dolorem delectus. Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nisi fugiat consequatur alias quia. Sed, tenetur repellendus sapiente ullam minima vero veritatis quasi officia, nesciunt dignissimos voluptate porro non repudiandae ea.",
  },
  {
    tab_title: "Backup",
    tab_content:
      "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Earum, iure maiores. Minima fugit repellendus velit quaerat dolores quo accusantium inventore, laudantium voluptate nulla ut illo tenetur adipisci hic suscipit repellat?",
  },
];

function changeTabLine(tabIndexValue) {
  active_tab.value = tabIndexValue;
}
</script>
