<template>
  <section id="members">
    <div class="members--wrapper">
      <h1 class="section--title">
        Thành viên tham gia
        <div class="member__title-line--separator"></div>
      </h1>
      <div class="members__carousel--wrapper">
        <MembersCarousel />
        <Members767 />
      </div>
    </div>
  </section>
</template>

<script>
import MembersCarousel from "./components/members-carousel.vue";
import Members767 from "./components/members-767.vue";

export default {
  name: "Memebers",
  components: {
    MembersCarousel,
    Members767,
  },
};
</script>

<style>
@import url("../../assets/member/common.css");
#carousel__768 {
  display: none !important;
}
#members {
  margin-top: 100px;
  width: 100%;
}
.members--wrapper {
  width: auto;
  height: 500px;
}
.section--title {
  margin-left: 123px !important;
}

.member__title-line--separator {
  margin-top: 8px;
  margin-left: 15px;
  width: 10vw;
  height: 4px;
  /* margin: auto; */
  background-image: linear-gradient(
    90deg,
    #4285f4 -19.99%,
    rgba(121, 220, 242, 0) 94.51%
  );
}

@media (max-width: 1399.98px) {
}
@media (max-width: 1199.98px) {
  .section--title {
    margin-left: 25px !important;
  }
}
@media (max-width: 991.98px) {
  .section--title {
    margin-left: 5px !important;
  }
  .members--wrapper {
    width: auto;
    height: 1040px;
  }
}
@media (max-width: 767.98px) {
  #carousel {
    display: none !important;
  }
  #carousel__768 {
    display: unset !important;
  }
  .section--title {
    margin-left: 20px !important;
  }
}

/* X-Small devices (portrait phones, less than 576px) */
@media (max-width: 575.98px) {
}

@media (max-width: 410.98px) {
  .member__title-line--separator {
    display: none !important;
  }
  .section--title {
    margin-left: 5px !important;
    font-size: 32px !important;
  }
}
@media (max-width: 410.98px) {
}
</style>