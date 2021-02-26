<template>
  <section id="home">
    <div class="home--wrapper" style="position: relative">
      <Navbar />
      <div class="home--content--wrapper" style="padding-top: 90px">
        <div
          class="home--content"
          data-aos="fade-up"
          data-aos-duration="1000"
          data-aos-delay="100"
        >
          <div class="home--title">
            <h1>
              <span style="color: #0b66bf">uniGO</span> - Hệ thống mô phỏng ảo
              bản đồ trường ĐH Bách Khoa - Đại học Đà Nẵng
            </h1>
          </div>
          <div class="home--text">
            <p>
              Sản phẩm được phát triển bởi Developer Student Clubs. Bằng cách áp
              dụng thuật toán cơ bản và các nền tảng công nghệ mới phổ biến,
              uniGO giúp người dùng tra cứu thông tin, địa điểm chính xác của
              các phòng học dễ dàng hơn.
            </p>
          </div>

          <Homebtn />
        </div>
        <div
          class="home--image"
          data-aos="fade-up"
          data-aos-duration="1000"
          data-aos-delay="400"
        >
          <img src="../../assets/home/img/home_bg.svg" alt="" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Homebtn from "./components/home-btn.vue";
export default {
  name: "home",
  components: {
    Navbar,
    Homebtn,
  },
  methods: {},
};
</script>

<style>
@import url("../../assets/home/common.css");

#home {
  width: 100%;
}
.home--content--wrapper {
  width: 100%;
  background: linear-gradient(180deg, #d2def5 0%, rgba(233, 240, 255, 0) 100%);
  display: flex;
}
.home--content {
  width: 50%;
  padding: 100px 0px 0px 11%;
}

.home--title {
  color: #202d51;
  line-height: 48px;
}
.home--title h1 {
  font-size: 35px;
  font-weight: 800;
}

.home--text {
  width: 100%;
  font-size: 20px;
  line-height: 27px;
  margin-top: 50px;
  color: #626262;
}

.home--image {
  margin-top: 11px;
  margin-left: 55px;
  width: 659px;
  height: auto;
}

@media (max-width: 1399.98px) {
  .home--content {
    padding: 60px 0px 0px 123px;
  }
  .home--text {
    width: 100%;
  }
  .home--image {
    width: 560px;
  }
}

/* Large devices (desktops, less than 1200px) */
@media (max-width: 1199.98px) {
  .home--content--wrapper {
    justify-content: space-between;
  }
  .home--content {
    width: 50%;
    padding: 55px 0px 0px 25px;
  }
  .home--image {
    width: 480px;
    margin-left: 0px;
    margin-right: 20px;
  }
}

/* Medium devices (tablets, less than 992px) */
@media (max-width: 991.98px) {
  .home--content--wrapper {
    justify-content: center;
  }
  .home--image {
    display: none;
  }
  .home--content {
    width: 80%;
    padding-left: 0;
  }
}

/* Small devices (landscape phones, less than 768px) */
@media (max-width: 767.98px) {
}

/* X-Small devices (portrait phones, less than 576px) */
@media (max-width: 575.98px) {
}

@media (max-width: 410.98px) {
}

@media (max-width: 321px) {
}
</style>