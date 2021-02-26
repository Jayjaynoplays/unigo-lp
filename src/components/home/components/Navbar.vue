<template>
  <div class="navbar--wrapper">
    <b-navbar
      toggleable="lg"
      type="dark"
      variant="dark"
      class="py-2 navbar--custom"
    >
      <b-navbar-brand href="#" class="navbar--logo">
        <img src="../../../assets/logo-text.svg" alt="logo-text" />
      </b-navbar-brand>

      <b-navbar-toggle
        target="nav-collapse"
        style="font-size: 1.25rem !important"
      ></b-navbar-toggle>

      <b-collapse class="ml_450" id="nav-collapse" is-nav>
        <b-navbar-nav class="navbar--underline navbar--text">
          <b-nav-item href="#" class="my-auto"> Trang chủ </b-nav-item>
          <b-nav-item href="#" class="my-auto">Tính năng</b-nav-item>
          <b-nav-item href="#" class="my-auto">Đối tượng sử dụng</b-nav-item>
          <b-nav-item href="#" class="my-auto">Q&A</b-nav-item>
          <b-nav-item href="#" class="my-auto">Thông tin liên hệ</b-nav-item>
          <b-nav-item href="#" class="my-auto">
            <Navbtn />
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
import Navbtn from "./Nav-btn.vue";
export default {
  name: "Navbar",
  components: {
    Navbtn,
  },
};
</script>

<style>
@import url("../../../assets/home/animation/Nav-underline.css");

.navbar {
  width: 100%;
}

.navbar-nav a {
  position: relative;
}
.navbar-nav li {
  margin-left: 14px;
}
.navbar-dark .navbar-nav .nav-link {
  text-decoration: none;
  font-weight: 600;
  font-size: 18px !important;
  color: #3e3e3e !important;
}

.navbar.navbar-dark.bg-dark {
  background-color: white !important;
  color: black;
}
.navbar-toggler-icon {
  background-image: url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'><path stroke='rgba(61, 61, 105, 1)' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/></svg>") !important;
}
.navbar-toggler {
  border-color: rgb(61, 61, 105) !important;
}

.ml_450 {
  margin-left: 350px;
  justify-content: center;
}

.navbar--wrapper {
  position: absolute;
  width: 100%;
  background: #ffffff;
  box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.1);
  z-index: 1300;
  display: flex;
  align-items: center;
}
.navbar--logo {
  margin-left: 10%;
}

.navbar--custom {
  box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.1);
}

@media (max-width: 1399.98px) {
  .navbar--logo {
    margin-left: 90px;
  }
  .ml_450 {
    margin-left: 160px;
  }
}

/* Large devices (desktops, less than 1200px) */
@media (max-width: 1199.98px) {
  .navbar--logo {
    margin-left: 0px;
  }
  .ml_450 {
    justify-content: flex-end;
    margin-left: 70px;
  }
  .navbar-nav li {
    margin-left: 0px;
  }
}

/* Medium devices (tablets, less than 992px) */
@media (max-width: 991.98px) {
  .ml_450 {
    margin-left: 45px;
    justify-content: flex-start;
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