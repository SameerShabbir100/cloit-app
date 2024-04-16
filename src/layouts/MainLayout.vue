<template>
  <q-layout view="lHh Lpr lFf">
    <TheHeader />
    <q-page-container class="q-pt-0">
      <router-view />
    </q-page-container>
    <TheFooter />
  </q-layout>
</template>

<script setup>
import TheHeader from "src/components/TheHeader.vue";
import TheFooter from "src/components/TheFooter.vue";

defineOptions({
  name: "MainLayout",
});
</script>

<style lang="sass" scoped>
.q-page-container
  padding-top: 0 !important
  padding-bottom: 0 !important
</style>
