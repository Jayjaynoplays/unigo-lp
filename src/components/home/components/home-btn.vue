<template>
  <div class="home--btn--wrapper">
    <a href="#">
      <button
        id="btn--try"
        class="btn--common btn--home btn--home--animation"
        ripple="ripple"
        @click="showPanel"
      >
        <div>Try uniGO</div>
        <div><em class="fas fa-arrow-down fa-2x"></em></div>
      </button>
    </a>

    <a href="#features">
      <button
        id="btn--discover"
        class="btn--common btn--home btn--home--animation"
        ripple="ripple"
      >
        <div>Discover</div>
        <div>
          <img
            src="../../../assets/home/img/discover.svg"
            alt="Khám Phá ngay"
          />
        </div>
      </button>
    </a>
  </div>
</template>

<script>
export default {
  name: "homeButton",
  methods: {
    showPanel() {
      this.$emit("show_panel");
    },
  },
};
</script>

<style>
@import url("../../../assets/home/common.css");

@import url("../../../assets/home/animation/homebtn.css");

a {
  text-decoration: none !important;
}

.home--btn--wrapper {
  margin-top: 100px;
}

.btn--home {
  width: 170px;
  height: 65px;
  position: relative;
  display: inline-block;
  overflow: hidden;
}

#btn--try {
  color: white;
  background-color: #0b66bf;
}
#btn--discover {
  margin-left: 25px;
  color: #626262;
  background-color: white;
}

@media (max-width: 1399.98px) {
  .home--btn--wrapper {
    margin-top: 50px;
  }
}

/* Large devices (desktops, less than 1200px) */
@media (max-width: 1199.98px) {
  .home--btn--wrapper {
    margin-top: 40px;
    margin-left: 0%;
  }
}

/* Medium devices (tablets, less than 992px) */
@media (max-width: 991.98px) {
  .home--btn--wrapper {
    display: flex;
    justify-content: center;
    padding-bottom: 1px;
  }
  #btn--try {
    margin-left: 0px;
  }
}

/* Small devices (landscape phones, less than 768px) */
@media (max-width: 767.98px) {
  #btn--try {
    margin-left: 25px;
  }
  #btn--discover {
    margin-left: 15px;
  }
}

/* X-Small devices (portrait phones, less than 576px) */
@media (max-width: 575.98px) {
}

@media (max-width: 410.98px) {
  .home--btn--wrapper a {
    display: flex;
    justify-content: center;
  }
  .btn--home {
    width: 145px;
    height: 55px;
  }
}

@media (max-width: 321px) {
}
</style>