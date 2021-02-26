<template>
  <div id="carousel" class="carousel slide" data-ride="carousel">
    <div class="position-relative" style="margin-top: 50px">
      <ol class="carousel-indicators">
        <li
          data-target="#carousel"
          data-slide-to="0"
          class="active department--name"
        >
          <div>
            <p>PM</p>
            <p>Project Manager</p>
          </div>
        </li>
        <li data-target="#carousel" data-slide-to="1" class="department--name">
          <div>
            <p>BA</p>
            <p>Business Analyst</p>
          </div>
        </li>
        <li data-target="#carousel" data-slide-to="2" class="department--name">
          <div>
            <p>UM</p>
            <p>UI/Map</p>
          </div>
        </li>
        <li data-target="#carousel" data-slide-to="3" class="department--name">
          <div>
            <p>FE</p>
            <p>Front-End</p>
          </div>
        </li>
        <li data-target="#carousel" data-slide-to="4" class="department--name">
          <div>
            <p>BA</p>
            <p>Back-End</p>
          </div>
        </li>
        <li data-target="#carousel" data-slide-to="5" class="department--name">
          <div>
            <p>Mo</p>
            <p>Mobile</p>
          </div>
        </li>
      </ol>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <b-row>
          <b-col>
            <img src="../../../assets/member/img/dung.svg" alt="Mạnh Dũng" />
            <p class="member--name center-text" style="margin-top: 4px">
              Phạm Mạnh Dũng
            </p>
          </b-col>
        </b-row>
      </div>

      <div class="carousel-item">
        <b-row class="row__responsive">
          <div :class="isColumn">
            <img
              src="../../../assets/member/img/linhhuong.svg"
              alt="Linh Hương"
            />
            <p class="member--name center-text">Nguyễn Linh Hương</p>
          </div>

          <div class="ml-55" :class="isColumn">
            <img src="../../../assets/member/img/mi.svg" alt="Duyên Trần" />
            <div class="member--name" id="duyen">
              <p class="center-text center-text">Trần Thị Thùy Duyên</p>
              <p class="department--name center-text" style="margin-top: -10px">
                BA-Lead
              </p>
            </div>
          </div>

          <div class="ml-55" :class="isColumn">
            <img
              src="../../../assets/member/img/nguyen.svg"
              alt="Nguyên Trần"
            />
            <p class="member--name center-text" style="margin-left: -20px">
              Trần Đình Phúc Nguyên
            </p>
          </div>
        </b-row>
      </div>

      <div class="carousel-item">
        <b-row class="row__responsive">
          <div :class="isColumn">
            <img src="../../../assets/member/img/oanh.svg" alt="Kim Oanh" />
            <p class="member--name center-text" style="margin-top: 2px">
              Đỗ Thị Kim Oanh
            </p>
          </div>

          <div class="ml-55" :class="isColumn">
            <img src="../../../assets/member/img/van.svg" alt="Tiến Văn" />
            <div class="member--name" style="margin-top: 4px">
              <p class="center-text center-text">Nguyễn Tiến Văn</p>
              <p class="department--name center-text" style="margin-top: -10px">
                Tech-Lead
              </p>
            </div>
          </div>

          <div class="ml-55" :class="isColumn">
            <img src="../../../assets/member/img/hai.svg" alt="Hải Lê" />
            <p class="member--name center-text" style="margin-top: 2px">
              Lê Hồng Hải
            </p>
          </div>
        </b-row>
      </div>

      <div class="carousel-item">
        <b-row style="justify-content: center">
          <b-col>
            <img
              style="padding: 0px"
              src="../../../assets/member/img/trumcuoi.svg"
              alt="Đức Huy"
            />
            <p class="member--name center-text" style="margin-top: 2px">
              Nguyễn Hữu Đức Huy
            </p>
            <p class="department--name center-text" style="margin-top: -10px">
              a.k.a Trùm-Cuối
            </p>
          </b-col>

          <b-col class="ml-55">
            <img
              src="../../../assets/member/img/lienhuong.svg"
              alt="Liên Hương"
            />
            <p class="member--name center-text" style="margin-top: 2px">
              Lê Liên Hương
            </p>
          </b-col>
        </b-row>
      </div>

      <div class="carousel-item">
        <b-row>
          <b-col>
            <img
              class="d-block"
              src="../../../assets/member/img/ichhoa.svg"
              alt="Ích Hòa"
            />
            <p class="member--name center-text" style="margin-top: 2px">
              Nguyễn ích Hòa
            </p>
          </b-col>
        </b-row>
      </div>

      <div class="carousel-item">
        <b-row>
          <b-col>
            <img
              class="d-block"
              src="../../../assets/member/img/duc.svg"
              alt="Nhân Đức"
            />
            <p class="member--name center-text" style="margin-top: 2px">
              Lê Vĩnh Nhân Đức
            </p>
          </b-col>
        </b-row>
      </div>
    </div>
    <div id="carousel_control">
      <a
        class="carousel-control-prev"
        data-target="#carousel"
        role="button"
        data-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a
        class="carousel-control-next"
        data-target="#carousel"
        role="button"
        data-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "MembersCarousel",
  data() {
    return {
      windowWidth: window.innerWidth,
    };
  },
  computed: {
    isColumn: function () {
      if (this.windowWidth <= 991.98) {
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
.col {
  min-height: unset !important;
}

.ml-55 {
  margin-left: 100px;
}
.carousel-item {
  height: 315px;
}
.row {
  width: 100%;
  justify-content: center;
  margin-left: 0px !important;
  margin-right: 0px !important;
}

.col {
  flex-grow: unset !important;
}

.carousel-indicators li {
  text-indent: unset !important;
  width: auto;
  height: auto;
  background-color: unset !important ;
  cursor: pointer;
  margin-left: 70px !important;
  width: auto !important;
  opacity: 1 !important;
}
.carousel-indicators {
  justify-content: unset !important;
  bottom: 0 !important;
  left: 0px !important ;
  top: -50px;
  margin-left: 0px !important;
  margin-right: 5% !important;
  display: -webkit-box !important;
}

.carousel-indicators .active {
  background-color: unset;
  color: #0b66bf;
}
.carousel-inner {
  top: 100px;
  left: 10% !important;
  width: 80% !important;
}

.carousel-control-prev {
  position: absolute;
  top: 120px !important;
  width: 3% !important;
  left: 120px !important;
}
.carousel-control-next {
  position: absolute;
  top: 120px !important;
  width: 3% !important;
  right: 115px !important;
}

.carousel-control-next-icon {
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='%23000' width='8' height='8' viewBox='0 0 8 8'%3e%3cpath d='M2.75 0l-1.5 1.5L3.75 4l-2.5 2.5L2.75 8l4-4-4-4z'/%3e%3c/svg%3e") !important;
}
.carousel-control-prev-icon {
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='%23000' width='8' height='8' viewBox='0 0 8 8'%3e%3cpath d='M5.25 0l-4 4 4 4 1.5-1.5L4.25 4l2.5-2.5L5.25 0z'/%3e%3c/svg%3e") !important;
}

@media (max-width: 1399.98px) {
  .carousel-indicators {
    margin-right: 0% !important;
    left: 0% !important;
  }
  .ml-55 {
    margin-left: 5vw !important;
  }
  .carousel-inner {
    left: 10% !important;
    width: 79% !important;
  }
  .carousel-indicators li {
    margin-left: 50px !important;
  }
  .carousel-control-prev {
    width: 2% !important;
  }
  .carousel-control-next {
    width: 2% !important;
    right: 130px !important;
  }
}

/* Large devices (desktops, less than 1200px) */
@media (max-width: 1199.98px) {
  .row {
    margin-left: 0 !important;
  }
  .carousel-inner {
    width: 92% !important;
    left: 4% !important;
  }
  .carousel-indicators {
    left: 0% !important;
  }
  .carousel-indicators li {
    margin-left: 40px !important;
  }
  .ml-55 {
    margin-left: 60px !important;
  }
  .carousel-control-prev {
    left: 25px !important;
  }
  .carousel-control-next {
    right: 25px !important;
  }
  #duyen {
    margin-left: -20px;
  }
}

/* Medium devices (tablets, less than 992px) */
@media (max-width: 991.98px) {
  .row__responsive {
    flex-direction: column;
    justify-content: center;
  }
  .name__center {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .carousel-inner {
    height: 868px;
  }
  .ml-55 {
    margin-left: 0px !important;
  }
  #carousel_control {
    display: none !important  ;
  }
  .carousel-indicators li:not(:first-child) {
    margin-left: 25px !important;
  }
  .carousel-indicators li:first-child {
    margin-left: 10px !important;
  }
  .memberPhoto__768 img {
    padding-left: 0 !important;
    margin-left: 20px !important;
  }
  .memberPhoto__768 .ml-55 {
    margin-left: 0;
  }
  .memberPhoto__768 img:first-child {
    margin-left: 0px !important;
  }
}
</style>