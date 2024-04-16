<template>
  <q-card flat class="footer-card bg-white q-pa-md q-mr-md">
    <q-card-section class="q-mb-sm q-pa-none">
      <img :src="props.icon" alt="Icon Code" width="40" height="40" />
    </q-card-section>

    <q-card-section
      class="title q-mb-md q-pa-none text-343741 fs-14 fw-9 lh-21"
    >
      {{ props.title }}
    </q-card-section>

    <q-card-section class="subtitle q-pa-none text-5E626F fs-14 fw-9 lh-21">
      <RouterLink to="/" class="flex text-decoration-none text-5E626F">
        {{ props.subtitle }}
        <span>
          <img
            src="src/assets/icon-arrow-next.svg"
            alt="Icon Arrow Next"
            width="20"
            height="20"
            class="arrow-next-icon q-ml-sm"
          />
        </span>
      </RouterLink>
    </q-card-section>
  </q-card>
</template>

<script setup>
const props = defineProps({
  icon: {
    type: String,
    default: "src/assets/icon-code.svg",
  },
  title: {
    type: String,
    default: "해외 개발자 원격 채용",
  },
  subtitle: {
    type: String,
    default: "바로가기",
  },
});
</script>

<style lang="sass" scoped>
.footer-card
  min-width: 187px
  height: 142px
  border-radius: 12px
  .text-5E626F
    color: #5E626F
  .text-343741
    color: #343741
  .text-decoration-none
    text-decoration: none

@media (max-width: 1300px)
  .footer-card
    min-width: 140px
    height: 120px
    margin-right: 12px
    padding: 12px
    img
      width: 30px
      height: 30px
    .title, .subtitle
      font-size: 12px
      line-height: 14px
    .title
      margin-bottom: 12px
    .subtitle
      .arrow-next-icon
        width: 16px
        height: 16px

@media (max-width: 577px)
  .footer-card
    min-width: 160px
    max-width: 160px
    height: 163px
    margin-right: 0
    img
      width: 40px
      height: 40px
    .title, .subtitle
      font-size: 14px
      line-height: 21px
    .title
      letter-spacing: -2px
      margin-bottom: 12px
    .subtitle
      .arrow-next-icon
        width: 20px
        height: 20px
</style>
