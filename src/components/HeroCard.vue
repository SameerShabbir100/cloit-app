<template>
  <q-card class="hero-card bg-white q-px-lg">
    <div class="flex items-center justify-center">
      <img
        src="src/assets/user-image.svg"
        alt="User"
        width="120"
        height="120"
      />
    </div>
    <h3 class="fs-24 fw-9 lh-36 text-black text-center q-mt-md q-mb-xs">
      {{ props.userName }}
    </h3>
    <p class="fs-16 fw-9 lh-24 text-4A77FF text-center q-mb-none">
      마케팅 · 2y+
    </p>
    <div class="text-center q-mt-lg">
      <q-badge
        outline
        label="마케팅 콘텐츠 제작"
        class="hero-badge text-5E626F q-py-xs q-px-sm fs-16 fw-9 lh-24"
      />
    </div>
    <div class="text-center q-mt-xs">
      <q-badge
        outline
        label="인스타그램 관리"
        class="hero-badge text-5E626F q-py-xs q-px-sm fs-16 fw-9 lh-24"
      />
    </div>
    <div class="text-center q-mt-xs">
      <q-badge
        outline
        label="트위터 관리"
        class="hero-badge text-5E626F q-py-xs q-px-sm q-mr-xs fs-16 fw-9 lh-24"
      />
      <q-badge
        outline
        label="블로그 글 작성"
        class="hero-badge text-5E626F q-py-xs q-px-sm fs-16 fw-9 lh-24"
      />
    </div>
    <q-tooltip
      anchor="top middle"
      self="bottom middle"
      :offset="[10, 10]"
      class="hero-card-tooltip bg-white text-secondary fs-18 fw-9 lh-27 q-px-md"
    >
      <q-badge
        rounded
        outline
        color="secondary"
        label="$"
        class="hero-badge text-secondary fs-16 fw-9 lh-24 q-pa-sm"
      />
      <strong>월 100만원</strong>
    </q-tooltip>
  </q-card>
</template>

<script setup>
const props = defineProps({
  userName: {
    type: String,
    default: "Abhishek Gupta",
  },
});
</script>

<style lang="sass" scoped>
.hero-card
  width: 292px
  min-height: 408px
  border-radius: 12px
  padding-top: 40px
  .text-4A77FF
    color: #4A77FF
  .text-5E626F
    color: #5E626F

@media (max-width: 1300px)
  .hero-card
    width: 250px
    min-height: 320px
    padding-top: 24px
    img
      width: 80px
      height: 80px
    h3
      font-size: 18px
      line-height: 24px
    p
      font-size: 14px
      line-height: 18px
    .hero-badge
      font-size: 12px
      line-height: 14px

@media (max-width: 770px)
  .hero-card
    width: 230px
    min-height: 280px
    padding-top: 12px
    img
      width: 60px
      height: 60px
    h3
      font-size: 16px
    p
      font-size: 12px
      line-height: 14px

@media (max-width: 775px)
  .hero-card
    width: 234px
    min-height: 312px
    padding-top: 24px
    padding-left: 12px
    padding-right: 12px
    img
      width: 64px
      height: 64px
    h3
      font-size: 18px
      line-height: 27px
    p, .hero-badge
      font-size: 14px
      line-height: 21px
    .hero-badge
      padding: 4px 8px
</style>
