<template>
  <nav aria-label="Page Navigation">
    <ul class="as-pagination">
      <li
        class="as-pagination__item"
        :class="{ 'as-pagination__item--disabled': currentPage == 1 }"
      >
        <button
          class="as-pagination__button"
          @click="clickHandler(currentPage - 1)"
          aria-label="Previous"
        >
          <i class="as-icon-arrow-left d-none d-lg-block"></i>
          <span class="as-text-12-semibold d-lg-none">Prev</span>
        </button>
      </li>
      <li class="as-pagination__item d-lg-none">
        <p class="as-text-12">{{ currentPage }}</p>
      </li>
      <li
        class="as-pagination__item d-none d-lg-flex"
        :class="{ 'as-pagination__item--active': page == currentPage }"
        v-for="page in pages"
        :key="page"
      >
        <i class="as-icon-dots" v-if="page == 'dots'"></i>
        <button
          class="as-pagination__button"
          @click="clickHandler(page)"
          v-else
        >
          {{ page }}
        </button>
      </li>
      <li
        class="as-pagination__item"
        :class="{
          'as-pagination__item--disabled': currentPage == totalPageCount,
        }"
      >
        <button
          class="as-pagination__button"
          @click="clickHandler(currentPage + 1)"
          aria-label="Next"
        >
          <i class="as-icon-arrow-right d-none d-lg-block"></i>
          <span class="as-text-12-semibold d-lg-none">Next</span>
        </button>
      </li>
    </ul>
  </nav>
</template>

<script setup>
import { computed, ref } from "vue";

const props = defineProps({
  currentPage: {
    default: 1,
    type: Number,
  },
  itemPerPage: {
    default: 10,
    type: Number,
  },
  siblingCount: {
    default: 1,
    type: Number,
  },
  totalCount: {
    required: true,
    type: Number,
  },
});

const emit = defineEmits(["pageChange"]);

const clickHandler = (page) => {
  currentPage.value = page;
  emit("pageChange", page);
};

const range = (start, end) => {
  const length = end - start + 1;
  return Array.from({ length }, (_, x) => start + x);
};

const currentPage = ref(props.currentPage);
const totalPageCount = ref(0);

const pages = computed(() => {
  totalPageCount.value = Math.ceil(props.totalCount / props.itemPerPage);

  const totalPageNumbers = props.siblingCount + 5;

  let result;

  if (totalPageNumbers >= totalPageCount.value) {
    result = range(1, totalPageCount.value);
  } else {
    const leftSiblingIndex = Math.max(
      currentPage.value - props.siblingCount,
      1
    );
    const rightSiblingIndex = Math.min(
      currentPage.value + props.siblingCount,
      totalPageCount
    );

    const shouldShowLeftDots = leftSiblingIndex > 2;
    const shouldShowRightDots = rightSiblingIndex < totalPageCount.value - 2;

    const firstPageIndex = 1;
    const lastPageIndex = totalPageCount.value;

    if (!shouldShowLeftDots && shouldShowRightDots) {
      let leftItemCount = 3 + 2 * props.siblingCount;
      let leftRange = range(1, leftItemCount);

      result = [...leftRange, "dots", totalPageCount.value];
    } else if (shouldShowLeftDots && !shouldShowRightDots) {
      let rightItemCount = 3 + 2 * props.siblingCount;
      let rightRange = range(
        totalPageCount.value - rightItemCount + 1,
        totalPageCount.value
      );

      result = [firstPageIndex, "dots", ...rightRange];
    } else if (shouldShowLeftDots && shouldShowRightDots) {
      let middleRange = range(leftSiblingIndex, rightSiblingIndex);
      result = [firstPageIndex, "dots", ...middleRange, "dots", lastPageIndex];
    }
  }

  return result;
});
</script>

<style lang="scss">
@use "@/assets/scss/components/pagination.scss";
</style>
