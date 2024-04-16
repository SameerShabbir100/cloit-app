<template>
  <q-header class="main-header bg-transparent q-pt-sm" reveal>
    <q-toolbar class="header-main-toolbar q-mx-auto q-px-xl justify-between">
      <div class="col-md-2">
        <img src="src/assets/logo.svg" alt="Logo" width="114" height="21" />
      </div>
      <div class="menu-section col-md-8">
        <div class="flex items-center justify-center">
          <div class="main-menu-btn cursor-pointer fs-16 fw-9 lh-24">
            채용
            <span class="q-ml-sm">
              <img
                src="src/assets/caret-down.svg"
                alt="Icon"
                width="16"
                height="16"
              />
            </span>
            <q-menu class="main-menu">
              <q-list style="min-width: 240px">
                <q-item clickable v-close-popup>
                  <q-item-section>채용</q-item-section>
                </q-item>
                <q-item clickable v-close-popup>
                  <q-item-section>해외 개발자 원격 채용</q-item-section>
                </q-item>
                <q-item clickable v-close-popup>
                  <q-item-section
                    >외국인 원격 채용 (비개발 직군)</q-item-section
                  >
                </q-item>
                <q-item clickable v-close-popup>
                  <q-item-section>한국어 가능 외국인 채용</q-item-section>
                </q-item>
              </q-list>
            </q-menu>
          </div>
          <RouterLink
            to="/about"
            class="any-page text-white q-ml-xl text-decoration-none fs-16 fw-9 lh-24"
          >
            해외 개발자 활용 서비스
          </RouterLink>
        </div>
      </div>
      <div class="sign-up-btn-section col-md-2 text-right">
        <q-btn
          color="white"
          class="sign-up-btn q-py-sm q-px-lg"
          to="/sign-up"
          unelevated
        >
          문의하기
        </q-btn>
      </div>
    </q-toolbar>
  </q-header>
</template>

<style lang="sass" scoped>
.main-header
  .header-main-toolbar
    max-width: 1440px
    .sign-up-btn
      color: #4A77FF !important
      border-radius: 8px
  .text-decoration-none
    text-decoration: none

@media (max-width: 770px)
  .main-header
    .header-main-toolbar
      width: 100%
      padding-left: 24px
      padding-right: 24px
      .main-menu-btn
        font-size: 14px
        line-height: 16px
        span
          margin-left: 8px
          img
            width: 14px
            height: 14px
        .main-menu
          font-size: 14px
          line-height: 16px
      .any-page
        font-size: 14px
        line-height: 16px
        margin-left: 16px
      .sign-up-btn
        font-size: 12px
        line-height: 14px
        padding: 4px 16px
        border-radius: 5px

@media (max-width: 577px)
  .main-header
    .header-main-toolbar
      padding-left: 12px
      padding-right: 12px
      .menu-section, .sign-up-btn-section
        display: none
</style>
