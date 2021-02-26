<template>
  <div id="carousel__768" class="carousel slide" data-ride="carousel">
    <div class="container position-relative">
      <a
        class="carousel-control-prev"
        data-target="#carousel__768"
        role="button"
        data-slide="prev"
        style="position: absolute; top: 170px; z-index: 1300"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a
        class="carousel-control-next"
        data-target="#carousel__768"
        role="button"
        data-slide="next"
        style="position: absolute; top: 170px; z-index: 1300"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>

    <div class="carousel-inner">
      <div class="carousel-item active">
        <div class="row">
          <div class="fl-cl">
            <p class="department--name center-text" style="margin-left: 7px">
              Project Manager
            </p>
            <img src="../../../assets/member/img/dung.svg" alt="Mạnh Dũng" />
            <div class="member--name" style="margin-top: 4px">
              <p class="center-text" style="margin-left: 15px">
                Phạm Mạnh Dũng
              </p>
            </div>
          </div>
        </div>
      </div>

      <div class="carousel-item">
        <div class="row">
          <div class="fl-cl">
            <p class="department--name center-text" style="margin-left: 0px">
              Business Analyst
            </p>

            <div class="ml-55" :class="is411">
              <img src="../../../assets/member/img/mi.svg" alt="Duyên Trần" />
              <div class="member--name" id="duyen">
                <p class="center-text">Trần Thị Thùy Duyên</p>
                <p
                  class="department--name center-text"
                  style="margin-left: -15px; margin-top: -15px"
                >
                  BA-Lead
                </p>
              </div>
            </div>

            <div class="ml-55" :class="is411">
              <img
                src="../../../assets/member/img/linhhuong.svg"
                alt="Linh Hương"
              />
              <div class="member--name">
                <p class="center-text" style="margin-right: 20px">
                  Nguyễn Linh Hương
                </p>
              </div>
            </div>

            <div class="ml-55" :class="is411">
              <img
                src="../../../assets/member/img/nguyen.svg"
                alt="Phúc Nguyên"
              />
              <div class="member--name">
                <p class="center-text" style="margin-left: -20px">
                  Trần Đình Phúc Nguyên
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="carousel-item">
        <div class="row">
          <div class="fl-cl">
            <p class="department--name center-text" style="margin-left: -6px">
              UI/Map
            </p>

            <div class="ml-55">
              <img src="../../../assets/member/img/van.svg" alt="Tiến Văn" />
              <div
                class="member--name"
                style="margin-top: -5px; margin-left: -15px"
              >
                <p class="center-text">Nguyễn Tiến Văn</p>
                <p
                  class="department--name center-text"
                  style="margin-left: -6px; margin-top: -15px"
                >
                  Tech-Lead
                </p>
              </div>
            </div>

            <div class="ml-55">
              <img src="../../../assets/member/img/hai.svg" alt="Hồng Hải" />
              <div class="member--name" style="margin-top: -5px">
                <p class="center-text">Lê Hồng Hải</p>
              </div>
            </div>

            <div class="ml-55">
              <img src="../../../assets/member/img/oanh.svg" alt="Kim Oanh" />
              <div class="member--name" style="margin-top: -5px">
                <p class="center-text">Đỗ Thị Kim Oanh</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="carousel-item">
        <div class="row">
          <div class="fl-cl">
            <p class="department--name center-text" style="margin-left: 0px">
              Front-End
            </p>

            <div class="ml-55">
              <img
                src="../../../assets/member/img/lienhuong.svg"
                alt="Liến Hương"
              />
              <div
                class="member--name"
                style="margin-top: 4px; margin-left: -20px"
              >
                <p class="center-text">Lê Liên Hương</p>
              </div>
            </div>

            <div class="ml-55">
              <img
                src="../../../assets/member/img/trumcuoi.svg"
                alt="Đức Huy"
              />
              <div class="member--name" style="margin-top: 4px">
                <p class="center-text">Nguyễn Hữu Đức Huy</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="carousel-item">
        <div class="row">
          <div class="fl-cl">
            <p class="department--name center-text" style="margin-left: -2px">
              Back-End
            </p>
            <div class="ml-55">
              <img src="../../../assets/member/img/ichhoa.svg" alt="Ích Hòa" />
              <div
                class="member--name"
                style="margin-top: 4px; margin-left: -20px"
              >
                <p class="center-text">Nguyễn ích Hòa</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="carousel-item">
        <div class="row">
          <div class="fl-cl">
            <p class="department--name center-text" style="margin-left: 0px">
              Mobile
            </p>
            <div class="ml-55">
              <img src="../../../assets/member/img/duc.svg" alt="Nhân Đức" />
              <div
                class="member--name"
                style="margin-top: 4px; margin-left: -20px"
              >
                <p class="center-text">Lê Vĩnh Nhân Đức</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Members767",
  data() {
    return {
      windowWidth: window.innerWidth,
    };
  },
  computed: {
    is411: function () {
      if (this.windowWidth <= 410.98) {
        return {
          name__center: true,
        };
      } else {
        return {
          name__center: false,
        };
      }
    },
  },
};
</script>

<style>
/* Small devices (landscape phones, less than 768px) */
@media (max-width: 767.98px) {
  #carousel {
    display: none;
  }
  #carousel__768 {
    display: unset;
  }

  .carousel-inner {
    height: 880px !important;
    top: 40px;
    width: 60% !important;
    left: 20% !important;
  }
  .carousel-control-prev {
    top: 53px !important;
  }
  .carousel-control-next {
    top: 53px !important;
  }
  .row img:not(:first-child) {
    padding-left: 35px !important;
  }
  .ml-55 {
    margin-left: 40px !important;
  }
  .carousel-control-prev {
    width: 3% !important;
  }
  .carousel-control-next {
    width: 3% !important;
  }
}

/* X-Small devices (portrait phones, less than 576px) */
@media (max-width: 575.98px) {
  .ml-55 {
    margin-left: 20px !important;
  }
  .carousel-inner {
    width: 86% !important;
    left: 7% !important;
    height: 920px !important;
  }
}

@media (max-width: 410.98px) {
  .ml-55 {
    margin-right: 5px !important;
  }
  .carousel-inner {
    height: 945px !important;
  }
  #duyen p:first-child {
    margin-left: 0px !important;
  }
}

@media (max-width: 321.98px) {
  .row img:not(:first-child) {
    padding-left: 0px !important;
  }
  .carousel-inner {
    width: 100% !important;
    left: 0% !important;
  }
}
</style>