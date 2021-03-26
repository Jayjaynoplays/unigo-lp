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
  .features__title--wrapper {
    width: 45%;
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
  .users h2 {
    text-align: center;
  }
  .users__title {
    width: 37vw;
    height: 8vw;
    border-radius: 6vw;
  }
  .announcement {
    top: 82vw !important;
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
    height: 107vw;
  }
  .info_1 {
    left: 10%;
    width: 41vw;
    top: 8vw;
  }
  .info_2 {
    right: 10%;
    width: 41vw;
    top: 36vw;
  }
  .pic1-bg {
    top: 0;
  }
  .pic2-bg {
    top: 30vw;
  }
  #features__school-event--text {
    top: 83vw;
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
    width: 330px;
  }
  #questions {
    margin-top: 100px;
  }
  .question__title--wrapper {
    width: 470px;
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
  .footer__form--wrapper {
    margin-left: 4vw;
  }
  .footer__form-subcribe--wrapper {
    width: 30vw;
    height: 4vw;
  }
  .footer__form--button {
    width: 40%;
  }
  .footer--wrap {
    height: 33vw;
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
    height: 175vw;
  }
  .features h3 {
    line-height: 5vw;
  }
  .features__title--wrapper {
    width: 65vw;
  }
  .info_1 {
    left: 4%;
    top: 5vw;
  }
  .info_1--img {
    width: 12%;
    margin-top: 5px;
  }
  .info_2 {
    top: 50vw;
    right: 4%;
  }
  .info_2--img {
    width: 12%;
    margin-top: 5px;
  }
  .pic1-bg {
    top: 0;
  }
  .pic2-bg {
    top: 50vw;
  }
  #features__room-info--text {
    top: 87vw;
  }
  .search {
    top: 90vw !important;
  }

  #features__school-event--text {
    top: 127vw;
  }
  .announcement {
    top: 134vw !important;
  }
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
  .question__title--wrapper {
    width: 75vw;
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
  .footer--wrap {
    height: 36vw;
  }
  .footer__form--input {
    font-size: 12px !important;
  }
  b {
    font-size: 15px !important;
  }
  .footer__form--wrapper {
    margin-left: 3vw;
  }
  .footer__form-subcribe--wrapper {
    width: 30vw;
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
    width: 100%;
    height: 33vw;
    margin-left: 1%;
  }
  .clubs-content,
  .guests--content {
    top: 95vw;
  }
  .clubs-content {
    left: 70% !important;
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
    height: 6vw;
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
  .features h3 {
    font-size: 20px !important;
    line-height: unset;
  }

  .features {
    margin-top: 0;
    height: 196vw;
  }
  .features__title--font p {
    font-size: 15px !important;
  }
  .info_1 {
    top: 0;
  }
  .pic1-bg {
    top: 0;
    left: 50%;
  }

  .pic1 {
    width: 45vw;
    height: auto;
  }
  .info_2 {
    top: 50vw;
    width: 45%;
    right: 5%;
  }
  .pic2-bg {
    top: 47vw;
    left: 2%;
  }
  .pic2 {
    width: 37vw;
    height: auto;
  }

  #features__room-info--text {
    top: 90vw;
  }
  .search {
    top: 95vw !important;
    left: 49% !important;
  }
  #features__school-event--text {
    top: 140vw !important ;
  }
  .announcement {
    top: 154vw !important;
    left: 5% !important;
  }
  .users__title--font {
    font-size: 15px !important;
  }
  .summary--bot {
    width: 125%;
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
  .features {
    height: 236vw;
    margin-top: 15px;
  }
  .clubs-content,
  .guests--content {
    top: 116vw;
  }
  .clubs-content {
    left: 68% !important;
  }
  .question__title--wrapper {
    width: 421px;
  }
  .info_2 {
    top: 60vw;
    right: 4%;
  }
  .pic2-bg {
    top: 58vw;
  }
  .pic2 {
    width: 184px;
  }
  #features__room-info--text {
    top: 110vw;
  }
  #features__school-event--text {
    top: 167vw !important;
  }
  .search {
    top: 113vw !important;
    left: 50% !important;
  }

  .users {
    height: 240vw;
  }
  .announcement {
    top: 180vw !important;
    left: 5% !important;
  }
  .clubs-content,
  .guests--content {
    top: 115vw;
  }

  .users h2 {
    margin-left: -12px;
  }
  .user__Students--description-summa {
    width: 110%;
  }
}

@media (max-width: 469.98px) {
  .features {
    height: 240vw;
  }
  .users {
    height: 236vw;
  }
  .clubs-content,
  .guests--content {
    top: 104vw;
  }
  .guests--content {
    left: 30%;
  }
  .lecturers-width {
    width: 25vw !important;
  }
  .users h2 {
    font-size: 22px;
  }
  .users__students--description-summary {
    font-size: 18px !important;
    width: 108%;
  }
}

@media (max-width: 449.98px) {
  .feature__title-line--separator {
    display: none;
  }
  .question__content--button {
    width: 15px;
    height: 15px;
    margin-right: 2vw;
  }
  .features {
    margin-top: 30px;
    height: 261vw;
  }
  .question__content--button2 {
    width: 15px;
    height: 15px;
    margin-right: 2vw;
  }
  .pic1-bg {
    width: 50vw;
    top: 5vw;
  }
  .pic2-bg {
    width: 50vw;
    top: 67vw;
  }
  .search {
    width: 50vw;
    top: 130vw !important;
  }
  .announcement {
    width: 50vw;
    top: 206vw !important;
  }
  .info_1 {
    left: 0%;
    top: 0;
    width: 50%;
  }
  .info_2 {
    right: 0%;
    width: 50%;
    top: 65vw;
  }
  #features__room-info--text {
    top: 119vw;
  }
  #features__school-event--text {
    top: 182vw !important;
  }
  .footer__contact-item--icon {
    width: 8px;
    height: 8px;
  }
  .users__title {
    width: 40vw;
    height: 12vw;
  }
  .users {
    height: 270vw;
  }
  .students {
    top: unset;
  }
  .freshman--content {
    top: unset;
  }
  .lecturers--content {
    top: unset;
  }

  .users__students--wrapper {
    top: 23vw;
  }
  .clubs-content,
  .guests--content {
    top: 135vw !important;
  }
  .freshman--content {
    left: 53%;
  }
  .clubs-content {
    left: 72% !important;
  }
  .summary--bot {
    width: 130% !important;
  }
  .guests--content {
    left: 25%;
  }

  .question__title-line--left,
  .feature__title-line--separator {
    height: 1px;
  }
  .question__title--wrapper {
    width: 393px;
    height: 11vw;
  }
  .question__item--wrapper,
  .question__item--wrapper2 {
    margin: auto;
    width: 70%;
  }
  .question__detail--wrapper,
  .question__detail--wrapper2 {
    height: 10vw;
  }
  .question__detail--font,
  .question__detail--font2 {
    margin-left: 2vw;
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
  .footer__contact-content--width {
    top: 42vw;
    justify-content: space-around;
    align-content: unset;
  }
  .footer__contact-item--wrapper {
    margin: 0;
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
  .footer__form-subcribe--wrapper {
    width: 45vw;
    height: 6vw;
  }
}

@media (max-width: 411.98px) {
  .features__title--description {
    font-size: 18px;
  }
  .features {
    margin-top: 70px;
    height: 303vw;
  }
  .info_1 {
    width: 55%;
  }
  .info_2 {
    top: 76vw;
    width: 55%;
  }
  .pic2-bg {
    left: 0%;
    top: 76vw;
  }
  #features__room-info--text {
    top: 147vw;
  }
  .search {
    top: 155vw !important;
    left: 55% !important;
  }
  .announcement {
    top: 245vw !important;
    left: -3% !important;
  }
  #features__school-event--text {
    top: 222vw !important;
  }

  .users {
    height: 1075px;
  }
  .users h2 {
    font-size: 20px;
  }
  .clubs-content {
    left: 78% !important;
  }
  .users__title {
    width: 45vw;
  }

  .question__title--wrapper {
    width: 100%;
  }
  .question__title-line--left {
    display: none;
  }
  .question__title-line--right {
    display: none;
  }
  .question__item--wrapper,
  .question__item--wrapper2 {
    width: 100%;
  }
  .question__detail--wrapper,
  .question__detail--wrapper2 {
    height: 15vw;
  }
  .question__detail--font,
  .question__detail--font2 {
    font-size: 16px !important;
  }
  .footer--wrap {
    height: 65vw;
  }
  .footer__logo {
    width: 30vw;
  }
  .footer__form--wrapper {
    left: 42vw;
  }
  .footer__contact-content--width {
    top: 57vw;
  }
  .footer__form-subcribe--wrapper {
    width: 49vw;
    height: 6vw;
  }
  .footer__link-sections {
    width: 38vw;
  }
  .phone {
    font-size: 10px !important;
  }
  .footer--button {
    right: 2vw;
    width: 8vw;
    height: 8vw;
  }
}

@media (max-width: 364.98px) {
  .features {
    height: 315vw;
  }
  .features__title--font h1 {
    font-size: 32px;
  }
  .question__title--font {
    font-size: 32px !important;
  }
  .features__title--description {
    margin-top: 10px;
  }
  .pic2-bg {
    top: 82vw;
  }
  .info_2 {
    top: 80vw;
  }
  .search {
    left: 52% !important;
  }

  .users {
    height: 320vw;
  }
  .users__title {
    width: 50vw;
    height: 15vw;
  }
  .users__students--wrapper {
    top: 30vw;
  }
  .clubs-content,
  .guests--content {
    top: 153vw !important;
  }
  .guests--content {
    left: 18%;
  }

  .question__content--button,
  .question__content--button2 {
    width: 17px;
    height: 17px;
    margin-right: 1vw;
  }
  .footer--wrap {
    height: 68vw;
  }
  .phone {
    width: 25vw;
  }
}

@media (max-width: 349.98px) {
  .features {
    margin-top: 90px;
    height: 251vw;
  }
  .pic1-bg {
    display: none;
  }
  .pic2-bg {
    display: none;
  }
  .search {
    display: none;
  }
  .announcement {
    display: none;
  }
  .info_1,
  .info_2 {
    width: 100%;
  }
  .info_2 {
    top: 57vw;
  }
  #features__room-info--text {
    top: 114vw;
  }
  #features__school-event--text {
    top: 181vw !important;
  }

  .users {
    height: 333vw;
  }
  .users__title {
    width: 60vw;
  }
  .users__students--description-summary {
    font-size: 15px !important;
  }
  .clubs-content,
  .guests--content {
    top: 155vw !important;
  }
  .clubs-content {
    left: 78% !important;
  }
  #clb--image-sm {
    margin-left: 10px;
  }

  .question__detail--font,
  .question__detail--font2 {
    font-size: 14px !important;
  }

  .footer--wrap {
    height: 69vw;
  }
  .footer__logo {
    width: 33vw;
  }
  .footer__contact-content--width {
    top: 60vw;
  }
  .phone {
    font-size: 9px !important;
  }
  .footer__form-subcribe--wrapper{
    width: 54vw;
  }
}
</style>
