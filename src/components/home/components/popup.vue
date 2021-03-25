<template>
  <div class="popup">
    <div class="popup__logo">
      <img src="../../../assets/logo-text.svg" alt="logo-text" />
    </div>
    <div class="popup__content--wrapper">
      <p class="text-common popup__content--text">
        uniGO is in development. Leave your email below to get latest news about
        our product. Subcribe
      </p>
    </div>
    <div class="popup__subcribes--wrapper">
      <input
        type="email"
        name="email"
        id="email"
        class="popup__subcribes--email"
        placeholder="example@email.com"
        @keyup.enter="submitEmail"
      />
      <a href="" class="popup__subcribes--button">
        <button @click="submitEmail" ripple="ripple">Subcribe</button>
      </a>
      <div class="popup__bottom--wrapper">
        <p class="text-common popup__bottom--text">
          Coming soon <br />
          ...
        </p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "popup",
  data() {
    return {
      panelResult: {},
    };
  },
  methods: {
    submitEmail() {
      alert("Email Submitted");
    },
  },
};
</script>
<style scoped>
@import url("../../../assets/home/animation/Nav-btn.css");

button :focus {
  outline: none !important;
}

input:focus {
  outline: none;
}
.text-common {
  font-family: "Nunito Sans";
  font-weight: 600;
  font-style: normal;
  text-align: center;
}
.popup {
  width: 100%;
  height: 100%;
  background: linear-gradient(180deg, #eaf1ff 0%, #ffffff 100%);
  display: flex;
  align-items: center;
  flex-direction: column;
}
.popup__logo {
  width: 283px;
  height: 100px;
  padding-top: 28px;
}
.popup__logo img {
  width: 100%;
}
.popup__content--wrapper {
  width: 551px;
  padding-top: 60px;
}
.popup__content--text {
  font-size: 24px;
  line-height: 33px;
  color: #202d51;
}

.popup__subcribes--wrapper {
  padding-top: 60px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.popup__subcribes--email {
  width: 327px;
  height: 48px;
  border: 1px solid #0a71c7;
  box-sizing: border-box;
  border-radius: 20px;
  padding-left: 10px;
}

::-webkit-input-placeholder {
  /* Edge */
  color: #bdbdbd;
  font-family: "Nunito Sans";
  font-size: 14px;
}

:-ms-input-placeholder {
  /* Internet Explorer */
  color: #bdbdbd;
  font-family: "Nunito Sans";
  font-size: 14px;
  margin-left: 10px;
}

::placeholder {
  color: #bdbdbd;
  font-family: "Nunito Sans";
  font-size: 14px;
  margin-left: 10px;
}

.popup__subcribes--button {
  margin-top: 15px;
}
.popup__subcribes--button button {
  background-color: #0b66bf;
  border-radius: 20px;
  border: none;
  width: 108px;
  height: 36px;
  color: white;
  cursor: pointer;
  font-size: 15px;
  line-height: 19px;
}
.popup__bottom--text {
  font-size: 18px;
  margin-top: 60px;
}
@media (max-width: 1399.98px) {
}

/* Large devices (desktops, less than 1200px) */
@media (max-width: 1199.98px) {
}

/* Medium devices (tablets, less than 992px) */
@media (max-width: 991.98px) {
}

/* Small devices (landscape phones, less than 768px) */
@media (max-width: 767.98px) {
  .popup__content--wrapper {
    width: 90%;
  }
}

/* X-Small devices (portrait phones, less than 576px) */
@media (max-width: 575.98px) {
  .popup__logo {
    width: 200px;
    height: auto;
  }
  .popup__subcribes--wrapper {
    padding-top: 40px;
  }
  .popup__subcribes--email {
    width: 277px;
    height: 48px;
  }
  .popup__bottom--text {
    margin-top: 60px;
  }
}

@media (max-width: 410.98px) {
  .popup__logo {
    width: 150px;
  }
  .popup__content--wrapper {
    padding-top: 30px;
  }
  .popup__content--text {
    font-size: 15px;
  }
  .popup__subcribes--wrapper {
    padding-top: 20px;
  }
  .popup__subcribes--email {
    width: 230px;
  }
  .popup__bottom--text {
    margin-top: 45px;
  }
}

@media (max-width: 321px) {
}
</style>