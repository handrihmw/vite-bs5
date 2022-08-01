<template>
  <div>
    <div class="row align-items-center">
      <AsAccordionSoft>
        <AsAccordionSoftTitle>
          <h3 class="as-text-16-bold">Accordion Title 1</h3>
        </AsAccordionSoftTitle>
        <AsAccordionSoftContent>
          <p class="as-text-14 as-color-secondary">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime
            mollitia fugit accusantium earum temporibus! Incidunt blanditiis
            cumque quisquam eius ipsa magnam optio, nulla inventore maxime sunt,
            reprehenderit est quia laudantium!
          </p>
        </AsAccordionSoftContent>
      </AsAccordionSoft>

      <AsAccordionSoft>
        <AsAccordionSoftTitle>
          <h3 class="as-text-16-bold">Accordion Title 2</h3>
        </AsAccordionSoftTitle>
        <AsAccordionSoftContent>
          <p class="as-text-14 as-color-secondary">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime
            mollitia fugit accusantium earum temporibus! Incidunt blanditiis
            cumque quisquam eius ipsa magnam optio, nulla inventore maxime sunt,
            reprehenderit est quia laudantium!
          </p>
        </AsAccordionSoftContent>
      </AsAccordionSoft>

      <AsAccordionSoft>
        <AsAccordionSoftTitle>
          <h3 class="as-text-16-bold">Accordion Title 3</h3>
        </AsAccordionSoftTitle>
        <AsAccordionSoftContent>
          <p class="as-text-14 as-color-secondary">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime
            mollitia fugit accusantium earum temporibus! Incidunt blanditiis
            cumque quisquam eius ipsa magnam optio, nulla inventore maxime sunt,
            reprehenderit est quia laudantium!
          </p>
        </AsAccordionSoftContent>
      </AsAccordionSoft>
    </div>
  </div>
</template>

<script setup>
import AsAccordionSoft from "./AsAccordionSoft.vue";
import AsAccordionSoftTitle from "./AsAccordionSoftTitle.vue";
import AsAccordionSoftContent from "./AsAccordionSoftContent.vue";

import { provide, reactive, ref, watch } from "vue";

let AccordionStatus = reactive({
  count: 0,
  active: null,
});

provide("AccordionStatus", AccordionStatus);
</script>
