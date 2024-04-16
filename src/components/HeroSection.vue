<template>
  <div class="hero-section">
    <div class="content-section q-mx-auto q-px-xl">
      <div class="row">
        <div class="col-12 col-sm-6">
          <h2 class="title text-white fs-48 fw-9 lh-62 q-mt-lg q-mb-none">
            최고의 실력을 가진
            <q-tooltip
              anchor="top middle"
              self="bottom middle"
              :offset="[10, 10]"
              class="hero-tooltip bg-white text-primary fs-18 fw-9 lh-27"
            >
              <strong>풀타임, 파트타임</strong>
            </q-tooltip>
            <span class="inline-block"> 외국인 인재를 찾고 계신가요? </span>
          </h2>
          <h5 class="subtitle text-white fs-24 fw-9 lh-34 q-mt-lg q-mb-lg">
            법률 및 인사관리 부담없이
            <span class="inline-block">
              1주일 이내에 원격으로 채용해보세요.
            </span>
          </h5>
          <h5 class="subtitle-mobile text-white fw-9">
            법률 및 인사관리 부담없이 1주일 이내에 원격으로 채용해보세요.
          </h5>
          <RouterLink
            class="redirect-to text-white fs-18 fw-9 lh-27"
            to="/contact-us"
          >
            개발자가 필요하신가요?
          </RouterLink>
          <div class="third-title flex justify-between q-mt-xl">
            <div class="third-title-section">
              <div class="upper-line q-mb-xs bg-white"></div>
              <h5 class="fs-18 fw-9 lh-27 text-white q-my-none">
                평균 월 120만원
              </h5>
              <h6 class="fs-14 fw-9 lh-24 text-white q-mt-sm q-mb-none">
                임금을 해당 국가를 기준으로 계산합니다.
              </h6>
            </div>
            <div class="third-title-section">
              <div class="upper-line q-mb-xs bg-white"></div>
              <h5 class="fs-18 fw-9 lh-27 text-white q-my-none">
                최대 3회 인력교체
              </h5>
              <h6 class="fs-14 fw-9 lh-24 text-white q-mt-sm q-mb-none">
                막상 채용해보니 맞지 않아도 걱정하지 마세요.
              </h6>
            </div>
            <div class="third-title-section">
              <div class="upper-line q-mb-xs bg-white"></div>
              <h5 class="fs-18 fw-9 lh-27 text-white q-my-none">
                평균 3일, 최대 10일
              </h5>
              <h6 class="fs-14 fw-9 lh-24 text-white q-mt-sm q-mb-none">
                급하게 사람이 필요한 경우에도 빠른 채용이 가능합니다.
              </h6>
            </div>
          </div>
        </div>
        <div class="col-12 col-sm-6">
          <q-carousel
            v-model="slide"
            transition-prev="scale"
            transition-next="scale"
            :transition-duration="200"
            animated
            infinite
            autoplay
            control-color="white"
            arrows
            height="420px"
            class="bg-transparent"
          >
            <q-carousel-slide name="slide-1" class="column no-wrap flex-center">
              <HeroCard user-name="Abhishek Gupta" />
            </q-carousel-slide>
            <q-carousel-slide name="slide-2" class="column no-wrap flex-center">
              <HeroCard user-name="Sahil Khan" />
            </q-carousel-slide>
            <q-carousel-slide name="slide-3" class="column no-wrap flex-center">
              <HeroCard user-name="Ranbir Kapoor" />
            </q-carousel-slide>
          </q-carousel>
        </div>
        <div class="checkboxes-section col-10">
          <q-checkbox
            v-model="checkboxOne"
            color="black"
            label="한국어 능력"
            class="text-white fs-16 fw-9 lh-24"
          />
          <q-checkbox
            v-model="checkboxTwo"
            color="black"
            label="업무 수행 능력"
            class="text-white fs-16 fw-9 lh-24"
          />
          <q-checkbox
            v-model="checkboxThree"
            color="black"
            label="겸업"
            class="text-white fs-16 fw-9 lh-24"
          />
          <q-checkbox
            v-model="checkboxFour"
            color="black"
            label="평판 조회"
            class="text-white fs-16 fw-9 lh-24"
          />
          <div>
            <RouterLink
              class="redirect-to-mobile text-FBFF23 fs-16 fw-9 lh-24 q-mt-sm"
              to="/contact-us"
            >
              개발자가 필요하신가요?
            </RouterLink>
          </div>
        </div>
      </div>
      <div
        class="hero-buttons-section flex items-center no-wrap q-pt-md q-mt-xl"
      >
        <HeroButton />
        <HeroButton icon="src/assets/icon-image.svg" text="퍼블리셔" />
        <HeroButton icon="src/assets/icon-box.svg" text="캐드원(제도사" />
        <HeroButton icon="src/assets/icon-target.svg" text="해외 세일즈" />
        <HeroButton icon="src/assets/icon-call.svg" text="퍼블리셔" />
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import HeroCard from "./HeroCard.vue";
import HeroButton from "./HeroButton.vue";

const slide = ref("slide-1");
const checkboxOne = ref(true);
const checkboxTwo = ref(true);
const checkboxThree = ref(true);
const checkboxFour = ref(true);
</script>

<style lang="sass" scoped>
.hero-section
  background-image: url("src/assets/hero-section-bg.svg")
  background-repeat: no-repeat
  background-size: cover
  background-position: center
  width: 100%
  min-height: 930px
  max-height: 930px
  .content-section
    max-width: 1440px
    padding-top: 200px
    .title
      width: 590px
      letter-spacing: -3px
    .subtitle
      width: 372px
      letter-spacing: -2px
    .subtitle-mobile
      display: none
    .third-title
      width: 590px
      .third-title-section
        width: 162px
        min-height: 92px
      .upper-line
        width: 130px
        height: 1px
    .hero-buttons-section
      width: 1390px
      overflow-x: hidden
    .checkboxes-section, .redirect-to-mobile
      display: none

@media (max-width: 1300px)
  .hero-section
    min-height: 750px
    max-height: 750px
    .content-section
      max-width: 100%
      padding-top: 150px
      .title
        width: 100%
        font-size: 38px
        line-height: 44px
        margin-top: 52px
      .subtitle
        width: 60%
        font-size: 18px
        line-height: 24px
      .redirect-to
        font-size: 14px
        line-height: 16px
      .third-title
        width: 100%
        .third-title-section
          width: 140px
          min-height: 72px
          h5
            font-size: 16px
            line-height: 24px
          h6
            font-size: 12px
            line-height: normal
        .upper-line
          width: 110px
      .hero-buttons-section
        width: 100%
        margin-top: 24px
        padding-top: 12px

@media (max-width: 770px)
  .hero-section
    min-height: 600px
    max-height: 600px
    .content-section
      padding-top: 80px
      padding-left: 24px
      padding-right: 24px
      .title
        font-size: 30px
        line-height: 36px
        margin-top: 44px
      .subtitle
        font-size: 16px
        line-height: 24px
      .third-title
        margin-top: 24px
        .third-title-section
          width: 100px
          min-height: 60px
          h5
            font-size: 14px
            line-height: 18px
        .upper-line
          width: 90px
      .hero-buttons-section
        width: 100%
        margin-top: 12px
        padding-top: 8px

@media (max-width: 577px)
  .hero-section
    background-image: url("src/assets/hero-section-bg-mobile.svg")
    min-height: 980px
    max-height: 980px
    .content-section
      padding-left: 12px
      padding-right: 12px
      .title
        font-size: 36px
        line-height: 47px
      .subtitle
        display: none
      .subtitle-mobile
        display: block
        font-size: 18px
        line-height: 27px
        margin-top: 24px
        margin-bottom: 48px
      .redirect-to, .third-title
        display: none
      .hero-buttons-section
        display: none
      .checkboxes-section, .redirect-to-mobile
        display: block
      .text-FBFF23
        color: #FBFF23
</style>
