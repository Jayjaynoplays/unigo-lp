<template>
  <section id="footer">
    <div class="footer--wrap" style="margin-top: 15vw">
      <div class="footer--wrapp-inner">
        <div class="footer__contact--wrapper">
          <img
            src="../assets/logouniGO-01.svg"
            class="footer__logo"
          />
          <div class="footer__contact-content--width">
            <div class="footer__contact-item--wrapper">
              <img
                src="../assets/Group (5).svg"
                class="footer__contact-item--icon"
              />
              <p class="footer__font-content">unigo@gmail.com</p>
            </div>
            <div class="footer__contact-item--wrapper">
              <img
                src="../assets/Vector.svg"
                class="footer__contact-item--icon"
              />
              <p class="footer__font-content">facebook.com/unigo</p>
            </div>
            <div class="footer__contact-item--wrapper">
              <img
                src="../assets/Vector (2).svg"
                class="footer__contact-item--icon"
              />
              <p
                class="footer__font-content phone"
                style="justify-content: left"
              >
                (+84) 915 469 728 <br /><span
                  >(Phạm Mạnh Dũng - Quản lý dự án)</span
                >
              </p>
            </div>
          </div>
        </div>
        <div class="footer__link-sections">
          <p class="footer__font-title">Liên kết nhanh</p>
          <div class="footer__links-item--wrapper">
            <img
              src="../assets/fast-forward 1.svg"
              class="footer__contact-item--icon"
            /><a href="#home" class="footer__font-content">Trang chủ</a>
          </div>
          <div class="footer__links-item--wrapper">
            <img
              src="../assets/fast-forward 1.svg"
              class="footer__contact-item--icon"
            /><a href="#features" class="footer__font-content">Tính năng</a>
          </div>
          <div class="footer__links-item--wrapper">
            <img
              src="../assets/fast-forward 1.svg"
              class="footer__contact-item--icon"
            /><a href="#user" class="footer__font-content">Đối tượng sử dụng</a>
          </div>
          <div class="footer__links-item--wrapper">
            <img
              src="../assets/fast-forward 1.svg"
              class="footer__contact-item--icon"
            /><a href="#questions" class="footer__font-content"
              >Các câu hỏi thường gặp</a
            >
          </div>
        </div>
        <div class="footer__form--wrapper">
          <p class="footer__font-title form-font">
            Bạn hãy để lại Gmail để nhận thông báo về ứng dụng sớm nhất nhé!
          </p>
          <div class="footer__form-subcribe--wrapper">
            <input
              placeholder="example@gmail.com"
              class="footer__form--input"
            /><button class="footer__form--button footer__font-content">
              Đăng kí
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style>
.footer__contact-content--width {
  margin-left: 6%;
  position: absolute;
  top: 6vw;
  left: 3%;
  width: 100%;
}
.footer--wrap {
  height: 20vw;
  width: auto;
  background-image: url("../assets/Rectangle\ 6.svg");
  background-size: cover;
  display: flex;
  color: #fff;
  padding: 1vw;
}
.footer__contact--wrapper {
  width: 35%;
  position: relative;
  left: 16%;
}
.footer__logo {
  width: 15vw;
  height: auto;
  position: absolute;
  top: -15%;
  left: 0;
}
.footer__font-title {
  font-weight: 800;
  font-size: 22px;
  margin: 0;
}
.footer__font-content {
  font-size: 16px;
  font-weight: 600;
  color: #fff;
  margin: 0;
}
.footer__links-item--wrapper a {
  color: #fff;
  text-decoration: none;
}
.footer__links-item--wrapper a:hover {
  text-decoration: underline !important;
  color: white;
}
.footer__contact-item--wrapper {
  display: flex;
  margin: 1vw 0 1vw 0;
  align-items: baseline;
}
.footer__links-item--wrapper {
  display: flex;
  margin: 1vw 0 1vw 0;
  align-items: center;
}
.footer__contact-item--icon {
  width: 15px;
  height: 15px;
  margin-right: 7px;
}
.footer__link-sections {
  width: 25%;
  margin-top: 6%;
  margin-right: 2vw;
  margin-left: 16vw;
}
.footer__form--wrapper {
  width: 10%;
  margin-top: 6%;
}
.footer__form-subcribe--wrapper {
  display: flex;
  width: 24vw;
  height: 3vw;
  border-radius: 3vw;
  border-style: solid;
  border-color: #0a71c7;
  margin-top: 25%;
}
.footer__form--input {
  width: 80%;
  color: #bdbdbd;
  font-weight: 600;
  font-size: 16px;
  background-color: transparent;
  border-top-left-radius: 3vw;
  border-bottom-left-radius: 3vw;
  margin-left: 1vw;
  border-color: transparent;
  outline: none;
}
::-moz-placeholder {
  color: #bdbdbd;
  font-weight: 600;
  font-size: 16px;
  align-items: center;
  justify-content: center;
}
:-ms-input-placeholder {
  color: #bdbdbd;
  font-weight: 600;
  font-size: 16px;
}
::placeholder {
  color: #bdbdbd;
  font-weight: 600;
  font-size: 16px;
}
.footer__form--button {
  background-color: #0b66bf;
  border-radius: 3vw;
  width: 30%;
  border-color: transparent;
  outline: none;
  cursor: pointer;
}
.form-font {
  width: 31vw;
}
.footer--button {
  outline: none;
  border: transparent;
  background-color: transparent;
  position: absolute;
  right: 4vw;
  cursor: pointer;
  width: 4vw;
  height: 4vw;
  background-color: #0b66c0;
  border-radius: 50%;
  box-shadow: 0 3px 6px rgba(0, 0, 0, 0.27058823529411763);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1000;
}
.footer--button-img {
  width: 2vw;
  height: 2vw;
}
.footer--wrapp-inner {
  display: flex;
  justify-content: center;
}
</style>