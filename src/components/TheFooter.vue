<template>
  <q-footer class="main-footer bg-FBFBFB q-py-lg q-px-xl">
    <div class="content-section q-mx-auto">
      <div class="main-row row q-pt-xl">
        <div class="col-sm-12 col-md-3 col-lg-4">
          <div class="logo-section">
            <img
              src="src/assets/footer-logo.svg"
              alt="Logo"
              width="187"
              height="34"
            />
            <p
              class="description text-343741 fs-14 fw-9 lh-21 q-mt-md q-mb-none"
            >
              우리는 국가의 장벽을 넘어 최고의 인재를 매칭해드립니다.
            </p>
            <p class="phone text-5E626F fs-13 fw-9 lh-20 q-mt-md q-mb-none">
              010-0000-0000
            </p>
            <p class="email text-5E626F fs-13 fw-9 lh-20 q-mt-md q-mb-none">
              aaaaa@naver.com
            </p>
            <div class="ceo-section flex justify-between items-center q-mt-xl">
              <p class="text-343741 fs-12 fw-9 lh-18 q-mb-none">상호명</p>
              <p class="text-343741 fs-12 fw-9 lh-18 q-mb-none">대표 CEO</p>
            </div>
            <div
              class="ceo-section-2 flex justify-between items-center q-mt-sm"
            >
              <p class="text-5E626F fs-13 fw-9 lh-20 q-mb-none">하이퍼하이어</p>
              <p class="text-5E626F fs-13 fw-9 lh-20 q-mb-none">김주현</p>
            </div>
            <div class="hyperhire flex justify-between items-center q-mt-sm">
              <p class="text-5E626F fs-12 fw-9 lh-20 q-mb-none">
                Hyperhire India Private Limited
              </p>
              <p class="text-5E626F fs-12 fw-9 lh-20 q-mb-none">Juhyun Kim</p>
            </div>
            <p class="copyright text-5E626F fs-13 fw-9 lh-20 q-mt-xl q-mb-none">
              &copy; 2023 Hyperhire
            </p>
          </div>
        </div>

        <div class="col-12 col-md-9 col-lg-8">
          <div class="footer-cards flex items-center">
            <FooterCard
              icon="src/assets/icon-code.svg"
              title="해외 개발자 원격 채용"
              subtitle="바로가기"
            />
            <FooterCard
              icon="src/assets/icon-avatar.svg"
              title="외국인 원격 채용 (비개발)"
              subtitle="바로가기"
            />
            <FooterCard
              icon="src/assets/icon-kor.svg"
              title="한국어 가능 외국인 채용"
              subtitle="바로가기"
            />
            <FooterCard
              icon="src/assets/icon-settings.svg"
              title="해외 개발자 활용 서비스"
              subtitle="바로가기"
            />
          </div>
          <div
            class="ceo-section-mobile flex justify-between items-center q-mt-xl"
          >
            <p class="text-343741 fs-12 fw-9 lh-18 q-mb-none">상호명</p>
            <p class="text-343741 fs-12 fw-9 lh-18 q-mb-none">대표 CEO</p>
          </div>
          <div
            class="ceo-section-2-mobile flex justify-between items-center q-mt-sm"
          >
            <p class="text-5E626F fs-13 fw-9 lh-20 q-mb-none">하이퍼하이어</p>
            <p class="text-5E626F fs-13 fw-9 lh-20 q-mb-none">김주현</p>
          </div>
          <div
            class="hyperhire-mobile flex justify-between items-center q-mt-sm"
          >
            <p class="text-5E626F fs-12 fw-9 lh-20 q-mb-none">
              Hyperhire India Private Limited
            </p>
            <p class="text-5E626F fs-12 fw-9 lh-20 q-mb-none">Juhyun Kim</p>
          </div>
          <div class="address-section flex items-center q-mt-xl">
            <div class="cin-section q-mr-xl">
              <p class="text-343741 fs-12 fw-9 lh-18 q-mb-sm">
                사업자등록번호 CIN
              </p>
              <p class="text-5E626F fs-13 fw-9 lh-20 q-mb-sm">427-86-01187</p>
              <p class="text-5E626F fs-13 fw-9 lh-20 q-mb-none">
                U74110DL2016PTC290812
              </p>
            </div>
            <div class="address-box">
              <p class="text-343741 fs-12 fw-9 lh-18 q-mb-sm">주소 ADDRESS</p>
              <p class="text-5E626F fs-13 fw-9 lh-20 q-mb-sm">
                서울특별시 강남대로 479, 지하 1층 238호
              </p>
              <p class="text-5E626F fs-13 fw-9 lh-20 q-mb-none">
                D-138, Street number 11, Jagjeet Nagar, North East Delhi, New
                Delhi, 110053 India
              </p>
            </div>
          </div>
          <p
            class="copyright-mobile text-5E626F fs-13 fw-9 lh-20 q-mt-xl q-mb-none"
          >
            &copy; 2023 Hyperhire
          </p>
        </div>
      </div>
    </div>
  </q-footer>
</template>

<script setup>
import FooterCard from "./FooterCard.vue";
</script>

<style lang="sass" scoped>
.bg-FBFBFB
  background-color: #FBFBFB
.main-footer
  height: 505px
  position: static
  .content-section
    max-width: 1440px
    .logo-section
      width: 285px
    .text-5E626F
      color: #5E626F
    .text-343741
      color: #343741
    .ceo-section-mobile, .ceo-section-2-mobile, .hyperhire-mobile
      display: none
    .address-box
      width: 455px
    .copyright-mobile
      display: none
@media (max-width: 1300px)
  .main-footer
    height: 400px
    padding-top: 12px
    padding-bottom: 12px
    .content-section
      width: 100%
      .main-row
        padding-top: 16px
        .footer-cards
          padding-left: 40px
        .address-section
          margin-top: 24px
          padding-left: 40px
          p
            font-size: 12px
            line-height: 14px
      .logo-section
        width: 100%
        img
          width: 160px
          height: auto
        .ceo-section, .copyright
          margin-top: 24px

@media (max-width: 770px)
  .main-footer
    height: auto
    padding-bottom: 12px
    padding-left: 24px
    padding-right: 24px
    .content-section
      .logo-section
        width: 600px
        margin-left: auto
        margin-right: auto
      .main-row
        .footer-cards
          margin-top: 24px
        .footer-cards, .address-section
          padding-left: 0
          justify-content: center
        .address-section
          .cin-section
            margin-right: 16px

@media (max-width: 577px)
  .main-footer
    height: auto
    padding-bottom: 12px
    padding-left: 12px
    padding-right: 12px
    .content-section
      .logo-section
        width: 247px
        img
          width: 187px
          height: auto
      .ceo-section, .ceo-section-2, .hyperhire, .copyright
        display: none
      .main-row
        .footer-cards
          margin-top: 16px
          column-gap: 10px
          row-gap: 10px
        .ceo-section-mobile, .ceo-section-2-mobile, .hyperhire-mobile
          display: flex
        .copyright-mobile
          display: block
        .address-section
          justify-content: start
          margin-top: 0
          .cin-section
            margin-right: 0
            margin-top: 40px
            margin-bottom: 40px
</style>
