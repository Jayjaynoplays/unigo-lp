<template>
  <div id="app">
    <Home />
    <Features />
    <Users />
    <Members />
    <Questions />
    <Footer />
  </div>
</template>

<script>
import Home from "./components/home/Home.vue";
import Features from "./components/Features.vue";
import Users from "./components/Users.vue";
import Members from "./components/members/Members.vue";
import Questions from "./components/Questions.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Home,
    Features,
    Users,
    Members,
    Questions,
    Footer,
  },
};
</script>

<style>
.section--title {
  font-family: "Nunito Sans";
  font-size: 35px;
  font-style: normal;
  font-weight: 800;
  line-height: 48px;
  letter-spacing: 0em;
  text-align: left;
  color: #0b66bf;
  /* margin-left: 225px; */
  display: flex;
  align-items: center;
}
* {
  font-family: Nunito Sans;
  margin: 0;
  padding: 0;
}

@media (max-width: 1399.98px) {
  .question__title--wrapper {
    width: 40vw;
  }
  .phone {
    width: 110%;
  }
  .users {
    height: 58vw;
  }
  /* * {
    font-size: 18px !important;
  } */
  .features__title--wrapper {
    width: 40%;
  }
  .features__title--font p {
    font-size: 29px !important;
  }
  .features {
    margin-top: 50px;
  }
  .info_1 {
    top: -50px;
  }
  .users__title--font {
    font-size: 22px !important;
  }
  /* .question__title--font {
    font-size: 29px !important;
  } */
  .features h3 {
    font-size: 20px !important;
  }
  #questions {
    margin-top: 100px;
  }
  .question__answer--detail,
  .question__detail--font,
  .question__detail--font2,
  b {
    font-size: 18px !important;
  }
  .footer__font-title {
    font-size: 20px;
  }
  .footer__font-content,
  .phone span {
    font-size: 18px !important;
  }
  .footer__link-sections {
    margin-top: 5%;
    width: 30%;
  }
  .footer__form--wrapper {
    margin-top: 5%;
  }
  .footer--wrap {
    height: 25vw;
  }
}

@media (max-width: 1199.98px) {
  /* * {
    font-size: 17px !important;
  } */
  .features {
    margin-top: 50px;
  }
  .info_1 {
    top: -60px;
  }
  .features__title--wrapper {
    height: 22vw;
    margin-left: 13px;
    width: 46%;
  }
  /* .features__title--font {
    font-size: 25px !important;
  } */
  .users {
    height: 65vw;
  }
  .users__title--font {
    font-size: 18px !important;
  }
  .question__title--wrapper {
    width: 48vw;
  }
  .question__title--font {
    width: 33vw;
  }
  /* .features__title--font p,
  .question__title--font {
    font-size: 25px !important;
  } */
  .features__title--font p {
    font-size: 25px !important;
  }
  .info_1 {
    left: 10%;
    width: 30vw;
  }
  .info_2 {
    right: 17%;
    width: 32vw;
  }
  .question__answer--detail,
  .question__detail--font,
  .question__detail--font2,
  b {
    font-size: 16px !important;
  }
  .question__answer--wrapper,
  .question__detail--wrapper,
  .question__detail--wrapper2 {
    width: 100%;
  }
  .footer__contact--wrapper {
    left: 0;
  }
  .footer__font-title {
    font-size: 15px !important;
  }
  .footer__link-sections {
    margin-left: 13vw;
  }
  .footer__form--wrapper {
    margin-left: 6vw;
  }
  .footer__font-content,
  .phone span {
    font-size: 13px !important;
  }
  ::-moz-placeholder {
    font-size: 13px !important;
  }
  :-ms-input-placeholder {
    font-size: 13px !important;
  }
  ::placeholder {
    font-size: 13px !important;
  }
}

@media (max-width: 991.98px) {
  .users__students--image {
    background-color: transparent;
  }
  /* * {
    font-size: 17px !important;
  } */
  .users h2 {
    text-align: center;
  }
  .users__title {
    width: 37vw;
    height: 8vw;
    border-radius: 6vw;
  }
  .announcement {
    top: 85vw !important;
    left: 12% !important;
  }
  .search {
    top: 54vw !important;
    left: 62% !important;
  }
  .lecturers-width {
    width: 20vw !important;
  }
  .users {
    height: 165vw;
    margin-top: 25vw;
  }
  .users__clubs--line,
  .users__freshman--line,
  .users__guests--line,
  .users__lecturers--line,
  .users__students--line {
    opacity: 0;
  }
  .features {
    background: transparent;
    margin-top: 50px;
    overflow-x: hidden;
    height: 114vw;
  }
  .info_1 {
    left: 10%;
    width: 41vw;
    top: 0;
  }
  .info_2 {
    right: 10%;
    width: 41vw;
  }
  .pic1-bg {
    top: 0;
  }
  .features__title--wrapper {
    height: 22vw;
    width: 58%;
    margin-left: 0px;
  }

  .features__title--font,
  .users__title--font {
    font-size: 25px !important;
  }
  .students {
    left: 16% !important;
    top: 15vw;
  }
  .users__img--shadow {
    position: relative;
  }
  .users__img--shadow,
  .users__students--image {
    width: 20vw;
    height: 20vw;
  }
  .users__img--circle {
    height: 17.5vw;
    width: 17.5vw;
  }
  .users__contents--wrapper {
    width: 20vw;
  }
  .freshman--content {
    top: 15vw;
    left: 50%;
    transform: translateX(-50%);
    border-color: #ff796a;
  }
  .lecturers--content {
    top: 15vw;
    left: 74vw;
    transform: translateX(-50%);
  }
  .guests--content {
    top: 80vw;
    left: 35%;
    transform: translateX(-50%);
  }
  .clubs-content {
    left: 62% !important;
    top: 80vw;
  }
  .question__title--font {
    /* font-size: 25px !important; */
    width: 330px;
  }
  #questions {
    margin-top: 100px;
  }
  .question__title--wrapper {
    width: 470px;
    /* height: 5vw; */
  }
  .question__answer--detail,
  .question__detail--font,
  .question__detail--font2,
  b {
    font-size: 13px !important;
  }
  .footer__font-title {
    font-size: 16px !important;
  }
  .footer__font-content,
  .phone span {
    font-size: 14px !important;
  }
  ::-moz-placeholder {
    font-size: 14px !important;
  }
  :-ms-input-placeholder {
    font-size: 14px !important;
  }
  ::placeholder {
    font-size: 14px !important;
  }
  .question__item--wrapper,
  .question__item--wrapper2 {
    padding: 2vw;
  }
  .footer__form-subcribe--wrapper {
    width: 27vw;
  }
  .footer__form--button {
    width: 40%;
  }
  .footer--wrap {
    height: 28vw;
  }
  .footer__logo {
    top: -8%;
  }
  .footer--button {
    right: 5vw;
    width: 5vw;
    height: 5vw;
  }
}

@media (max-width: 767.98px) {
  .question__content--button,
  .question__content--button2 {
    width: 18px;
    height: 18px;
  }
  .features {
    height: 156vw;
  }
  .info_1 {
    left: 4%;
    top: 0;
  }
  .info_2 {
    top: 40vw;
  }
  .pic1-bg {
    top: 0;
  }
  .pic2-bg {
    top: 42vw;
  }
  #features__room-info--text {
    top: 75vw;
  }
  .search {
    top: 77vw !important;
  }
  .features__title--wrapper {
    width: 65vw;
    /* height: 30vw; */
  }

  #features__school-event--text {
    top: 113vw;
  }
  .announcement {
    top: 124vw !important;
  }

  /* *,
  .features h3 {
    font-size: 15px !important;
  } */
  .features__title--font p,
  .users__title--font {
    font-size: 20px !important;
  }
  .users__contents--wrapper {
    width: 27vw;
  }
  .users__title {
    width: 38vw;
    height: 8vw;
  }
  .guests--content {
    top: 85vw;
    left: 28%;
  }
  .clubs-content {
    left: 68% !important;
    top: 86vw;
  }
  .users {
    height: 190vw;
    margin-top: 17vw;
  }
  .students {
    left: 6% !important;
  }
  .lecturers--content {
    left: 85vw;
  }

  /* .question__title--font {
    font-size: 20px !important;
  } */
  .question__title--wrapper {
    width: 75vw;
    /* height: 7vw; */
  }
  .question__content--wrapper {
    display: block;
  }
  .question__item--wrapper,
  .question__item--wrapper2 {
    margin: auto;
    width: 63%;
  }
  .question__answer--wrapper {
    width: 100%;
  }
  .question__detail--wrapper,
  .question__detail--wrapper2 {
    height: 6vw;
  }
  .footer__font-title {
    font-size: 12px !important;
  }
  .footer__font-content,
  .phone span {
    font-size: 11px !important;
  }
  ::-moz-placeholder {
    font-size: 11px !important;
  }
  :-ms-input-placeholder {
    font-size: 11px !important;
  }
  ::placeholder {
    font-size: 11px !important;
  }
  .question__answer--detail,
  .question__detail--font,
  .question__detail--font2 {
    font-size: 15px !important;
  }
  .footer__form--input {
    font-size: 12px !important;
  }
  b {
    font-size: 15px !important;
  }
  .footer__form-subcribe--wrapper {
    width: 29vw;
  }
  .button-up {
    top: 92%;
  }
  .footer__contact-item--icon {
    width: 11px;
    height: 11px;
  }
}

@media (max-width: 575.98px) {
  .features__title--wrapper {
    width: 62vw;
    height: 33vw;
    margin-left: 10%;
  }

  .clubs-content,
  .guests--content {
    top: 71vw;
  }
  .footer--wrapp-inner {
    position: relative;
  }
  .footer__logo {
    width: 21vw;
    top: 0;
    left: 9vw;
  }
  .footer__link-sections {
    position: absolute;
    top: 27%;
    left: 11vw;
    width: 35vw;
    margin: 0;
  }
  .form-font {
    width: 45vw;
  }
  .footer__form-subcribe--wrapper {
    width: 38vw;
    height: 5vw;
    margin-top: 2vw;
  }
  .footer__form--wrapper {
    position: absolute;
    top: 27%;
    width: 100%;
    left: 48vw;
  }
  .footer__contact-content--width {
    width: 100vw;
    position: absolute;
    top: 35vw;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .footer__contact-item--wrapper {
    display: flex;
    margin: 5vw 2vw 1vw 7vw;
    justify-content: center;
    align-items: center;
  }
  .footer__contact-item--icon {
    margin-right: 1vw;
  }

  *,
  .features h3 {
    font-size: 12px !important;
  }

  .features {
    margin-top: 0;
  }
  .features__title--font p {
    font-size: 15px !important;
  }
  .info_1 {
    top: 0;
  }
  .pic1-bg {
    top: 0;
  }
  .info_2 {
    top: 40vw;
    width: 45%;
  }
  .pic2-bg {
    top: 44vw;
  }

  #features__room-info--text {
    top: 70vw;
  }
  #features__room-info--image {
    top: 70vw !important ;
  }
  /* .question__title--font, */
  .users__title--font {
    font-size: 15px !important;
  }
  .footer__font-content {
    font-size: 8px !important;
    justify-content: center;
    align-items: center;
    display: flex;
  }
  .question__answer--detail,
  .question__detail--font,
  .question__detail--font2,
  b {
    font-size: 12px !important;
  }
  .footer--wrap {
    padding: 0;
    height: 50vw;
  }
  .footer__font-title {
    font-size: 12px !important;
  }
  .footer__font-content {
    font-size: 11px !important;
  }
  ::-moz-placeholder {
    font-size: 11px !important;
  }
  :-ms-input-placeholder {
    font-size: 11px !important;
  }
  ::placeholder {
    font-size: 11px !important;
  }
  .question__title-line--left,
  .feature__title-line--separator {
    height: 2px;
  }
  .phone span {
    opacity: 0;
    font-size: 0 !important;
  }
  .phone {
    width: 24vw;
  }
  p.footer__font-content.phone:hover {
    z-index: 2000;
  }
  .contact {
    opacity: 0;
  }
  .question__title-line--left,
  .feature__title-line--separator {
    width: 7vw;
  }
  .question__title--wrapper {
    width: 80vw;
    height: 9vw;
  }
}

@media (max-width: 525.98px) {
  .clubs-content,
  .guests--content {
    top: 82vw;
  }
  .question__title--wrapper {
    width: 421px;
    /* height: 9vw; */
  }
}

@media (max-width: 469.98px) {
  .clubs-content,
  .guests--content {
    top: 84vw;
  }
}

@media (max-width: 449.98px) {
  .question__content--button {
    width: 15px;
    height: 15px;
    margin-right: 2vw;
  }
  .info_1 {
    width: 43vw;
  }
  .question__content--button2 {
    width: 15px;
    height: 15px;
    margin-right: 2vw;
  }
  .features h3 {
    font-size: 9px !important;
  }
  .features__title--description {
    font-size: 10px !important;
  }
  .pic2-bg {
    left: 12%;
  }
  * {
    font-size: 10px !important;
  }
  .info_1 {
    left: 9%;
    top: 0;
  }
  .info_2 {
    right: 9%;
  }
  .footer__contact-item--icon {
    width: 8px;
    height: 8px;
  }
  .features__title--font p {
    font-size: 15px !important;
  }
  .users__title {
    width: 34vw;
    height: 8vw;
  }
  .users__title--font {
    font-size: 10px !important;
  }
  .clubs-content,
  .guests--content {
    top: 78vw;
  }
  .users {
    height: 175vw;
  }
  .question__title-line--left,
  .feature__title-line--separator {
    height: 1px;
  }
  /* .question__title--font {
    font-size: 15px !important;
  } */
  .question__title--wrapper {
    width: 393px;
    height: 11vw;
  }
  .question__item--wrapper,
  .question__item--wrapper2 {
    margin: auto;
    width: 63%;
  }
  .question__detail--font,
  .question__detail--font2 {
    font-size: 9px !important;
    margin-left: 2vw;
  }
  .footer__font-title,
  .question__answer--detail,
  b {
    font-size: 9px !important;
  }
  .footer__font-content {
    font-size: 8px !important;
  }
  .footer__logo {
    width: 25vw;
    left: 0;
  }
  .footer__link-sections {
    top: 32%;
    left: 2vw;
  }
  .footer__form--wrapper {
    top: 37%;
    margin-left: 0;
    left: 40vw;
  }
  ::-moz-placeholder {
    font-size: 8px !important;
  }
  :-ms-input-placeholder {
    font-size: 8px !important;
  }
  ::placeholder {
    font-size: 8px !important;
  }
  .form-font {
    width: 50vw;
  }
  .question__title-line--left,
  .feature__title-line--separator {
    width: 9vw;
  }
  .features__title--font {
    height: 32%;
  }
}

@media (max-width: 412px) {
  .question__title--wrapper{
    width: 100%;
  }
  .question__title-line--left {
    display: none;
  }
  .question__title-line--right {
    display: none;
  }
  * {
    font-size: 9px !important;
  }
}

@media (max-width: 364.98px) {
  .question__content--button,
  .question__content--button2 {
    width: 12px;
    height: 12px;
    margin-right: 2vw;
  }
  * {
    font-size: 8px !important;
  }
  .clubs-content,
  .guests--content {
    top: 73vw;
  }
  .footer__contact-content--width {
    top: 38vw;
  }
  .question__item--wrapper,
  .question__item--wrapper2 {
    margin: auto;
    width: 68%;
  }
  .question__title--font{
    width: 100%;
    font-size: 33px !important;
  }
}

@media (max-width: 349.98px) {
  .clubs-content,
  .guests--content {
    top: 81vw;
  }
}
</style>
