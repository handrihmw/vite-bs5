<template>
  <div>
    <div class="row align-items-center">
      <AsAccordion>
        <AsAccordionTitle>
          <h3 class="as-text-16">Accordion Title 1</h3>
        </AsAccordionTitle>
        <AsAccordionContent>
          <p class="as-text-14 as-color-secondary-2">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime
            mollitia fugit accusantium earum temporibus! Incidunt blanditiis
            cumque quisquam eius ipsa magnam optio, nulla inventore maxime sunt,
            reprehenderit est quia laudantium!
          </p>
        </AsAccordionContent>
      </AsAccordion>

      <AsAccordion>
        <AsAccordionTitle>
          <h3 class="as-text-16">Accordion Title 2</h3>
        </AsAccordionTitle>
        <AsAccordionContent>
          <p class="as-text-14 as-color-secondary-2">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime
            mollitia fugit accusantium earum temporibus! Incidunt blanditiis
            cumque quisquam eius ipsa magnam optio, nulla inventore maxime sunt,
            reprehenderit est quia laudantium!
          </p>
        </AsAccordionContent>
      </AsAccordion>

      <AsAccordion>
        <AsAccordionTitle>
          <h3 class="as-text-16">Accordion Title 3</h3>
        </AsAccordionTitle>
        <AsAccordionContent>
          <p class="as-text-14 as-color-secondary-2">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime
            mollitia fugit accusantium earum temporibus! Incidunt blanditiis
            cumque quisquam eius ipsa magnam optio, nulla inventore maxime sunt,
            reprehenderit est quia laudantium!
          </p>
        </AsAccordionContent>
      </AsAccordion>
    </div>
  </div>
</template>

<script setup>
import AsAccordion from "./AsAccordion.vue";
import AsAccordionTitle from "./AsAccordionTitle.vue";
import AsAccordionContent from "./AsAccordionContent.vue";

import { provide, reactive, ref, watch } from "vue";

let AccordionStatus = reactive({
  count: 0,
  active: null,
});

provide("AccordionStatus", AccordionStatus);
</script>
