<template>
  <section class="as-section-white as-py-48 as-px-20">
    <div class="as-section__container">
      <h2 class="as-section__title as-mb-32 text-lg-center">
        Our Recruitment Process
      </h2>
      <p class="as-section__description as-mb-32 text-lg-center">
        Our recruitment process takes up around two weeks in average depending
        on the nature of the job position. However, in general, you will have to
        go through the following stages:
      </p>

      <ul class="recruitment-card-wrapper">
        <li
          class="as-recruitment-card-v2 as-card__container--xxlg"
          v-for="item in dataRecruitmentV2"
          :key="item.id"
        >
          <img
            :src="item.src"
            alt="recruitment process 1"
            class="as-recruitment-card-v2__image"
          />
          <h3 class="as-text-20-bold as-color-primary as-lh-26 as-mb-18">
            {{ item.title }}
          </h3>
          <p class="as-text-16 as-color-secondary as-lh-24">
            {{ item.description }}
          </p>
        </li>
      </ul>
    </div>
  </section>
</template>

<script setup>
import imgRec1 from "@/assets/images/samples/organism/lpkarir/recruitment-1.svg";
import imgRec2 from "@/assets/images/samples/organism/lpkarir/recruitment-2.svg";
import imgRec3 from "@/assets/images/samples/organism/lpkarir/recruitment-3.svg";
import imgRec4 from "@/assets/images/samples/organism/lpkarir/recruitment-4.svg";
import imgRec5 from "@/assets/images/samples/organism/lpkarir/recruitment-5.svg";
import imgRec6 from "@/assets/images/samples/organism/lpkarir/recruitment-6.svg";

const dataRecruitmentV2 = [
  {
    src: imgRec1,
    title: "Online Application",
    description:
      "Apply through our Career Page or external job portals that’s officially posted by Niagahoster.",
  },
  {
    src: imgRec2,
    title: "Technical test",
    description:
      "You’ll have to work on a test related to the applied position to prove your skills and capabilities.",
  },
  {
    src: imgRec3,
    title: "HR interview",
    description:
      "Be transparent in sharing your qualifications and personal values. You’ll also learn more about ours!",
  },
  {
    src: imgRec4,
    title: "Psychometric test",
    description:
      "Your logical thinking and personality traits will be revealed in this process. Be fully focused!",
  },
  {
    src: imgRec5,
    title: "User interview",
    description:
      "Meet your future teammates who will dive deep into your technical skills and experiences!",
  },
  {
    src: imgRec6,
    title: "Job offering",
    description:
      "If you are the chosen one, the job will be yours. Finally, welcome to your new home, Hoster Ranger!",
  },
];
</script>

<style lang="scss">
@use "@/assets/scss/mixins/breakpoint" as *;
.as-section-white {
  @include screen(desktop) {
    padding-block: 3.75rem;
  }

  .as-section__title,
  .as-section__description {
    @include screen(desktop) {
      max-width: 57.5rem;
      margin-inline: auto;
    }
  }

  .recruitment-card-wrapper {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    @include screen(desktop) {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 3rem;
      margin-top: 3.75rem;
    }
  }
}
</style>
