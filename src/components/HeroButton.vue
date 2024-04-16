<template>
  <q-btn
    class="hero-button q-pa-md q-mr-sm items-start fs-24 fw-9 lh-36"
    text-color="white"
    unelevated
  >
    <img :src="props.icon" alt="Icon" class="q-mr-md" width="56" height="56" />
    {{ props.text }}
  </q-btn>
</template>

<script setup>
const props = defineProps({
  icon: {
    type: String,
    default: "src/assets/icon-marketing.svg",
  },
  text: {
    type: String,
    default: "해외 마케팅",
  },
});
</script>

<style lang="sass" scoped>
.hero-button
  min-width: 332px
  height: 88px
  border-radius: 12px
  background-color: #FFFFFF33

@media (max-width: 1300px)
  .hero-button
    min-width: 250px
    height: auto
    font-size: 16px
    line-height: 24px
    img
      width: 48px
      height: 48px

@media (max-width: 1200px)
  .hero-button
    min-width: 200px
    height: auto
    font-size: 16px
    line-height: 24px
    img
      width: 44px
      height: 44px

@media (max-width: 770px)
  .hero-button
    min-width: 150px
    font-size: 14px
    line-height: 18px
    padding: 8px
    border-radius: 8px
    img
      width: 20px
      height: 20px
</style>
