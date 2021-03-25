<template>
  <section id="questions">
    <div class="question--wrapper">
      <div class="question__title--wrapper">
        <div class="question__title-line--left"></div>
        <div class="question__title--font">Câu hỏi thường gặp</div>
        <div class="question__title-line--right"></div>
      </div>
      <div class="question__content--wrapper">
        <div class="question__item--wrapper">
          <button
            :class="isAnswer0 ? wrapper2 : wrapper"
            @click="changeStatus0"
          >
            <div class="question__detail">
              <p :class="isAnswer0 ? font2 : font">
                What is the purpose of uniGO?
              </p>
              <div :class="isAnswer0 ? button2 : button">
                <i class="fas fa-plus" :class="isAnswer0 ? icon2 : icon"></i>
              </div>
            </div>
          </button>
          <div
            class="question__answer--wrapper"
            :style="isAnswer0 ? height2 : height"
          >
            <div class="question__answer--detail">
              <b>uniGO</b> ra đời với mong muốn xây dựng và đóng góp vào cộng
              đồng. Được mọi người đón nhận và từng bước ứng dụng trong thực
              tiễn.
            </div>
          </div>
        </div>
        <div class="question__item--wrapper">
          <button
            :class="isAnswer1 ? wrapper2 : wrapper"
            @click="changeStatus1"
          >
            <div class="question__detail">
              <p :class="isAnswer1 ? font2 : font">What is DSC-DUT?</p>
              <div :class="isAnswer1 ? button2 : button">
                <i class="fas fa-plus" :class="isAnswer1 ? icon2 : icon"></i>
              </div>
            </div>
          </button>
          <div
            class="question__answer--wrapper"
            :style="isAnswer1 ? height2 : height"
          >
            <div class="question__answer--detail">
              <b
                >DSC - DUT (Developer Student Clubs - Da Nang University of
                Science and Technology)</b
              >
              là cộng đồng do Google Developers bảo trợ. Gồm các bạn sinh viên
              trẻ năng động đến từ các trường đại học trực thuộc đại học Đà
              Nẵng, quan tâm tới việc xây dựng và đưa ra các giải pháp phát
              triển cộng đồng.
            </div>
          </div>
        </div>
        <div class="question__item--wrapper">
          <button
            :class="isAnswer2 ? wrapper2 : wrapper"
            @click="changeStatus2"
          >
            <div class="question__detail">
              <p :class="isAnswer2 ? font2 : font">
                Do I need to pay to install uniGO?
              </p>
              <div :class="isAnswer2 ? button2 : button">
                <i class="fas fa-plus" :class="isAnswer2 ? icon2 : icon"></i>
              </div>
            </div>
          </button>
          <div
            class="question__answer--wrapper"
            :style="isAnswer2 ? height2 : height"
          >
            <div class="question__answer--detail">
              <b>Hoàn toàn không.</b> Đây là sản phẩm phi lợi nhuận được phát
              triển bởi DSC - DUT cho đơn vị trường Đại học Bách Khoa, hỗ trợ
              tra cứu thông tin địa điểm nhanh chóng và chính xác.
            </div>
          </div>
        </div>
        <div class="question__item--wrapper">
          <button
            :class="isAnswer3 ? wrapper2 : wrapper"
            @click="changeStatus3"
          >
            <div class="question__detail">
              <p :class="isAnswer3 ? font2 : font">
                Does this app require Internet connection?
              </p>
              <div :class="isAnswer3 ? button2 : button">
                <i class="fas fa-plus" :class="isAnswer3 ? icon2 : icon"></i>
              </div>
            </div>
          </button>
          <div
            class="question__answer--wrapper"
            :style="isAnswer3 ? height2 : height"
          >
            <div class="question__answer--detail">
              Hiện tại, sản phẩm sẽ được thiết kế dùng trước trên website và mở
              rộng ra điện thoại. Trước mắt, các thiết bị sẽ yêu cầu
              <b>có kết nối internet</b> (3G/4G/Wifi) để có thể sử dụng.
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "Questions",
  data() {
    return {
      isAnswer0: false,
      isAnswer1: false,
      isAnswer2: false,
      isAnswer3: false,
      font: "question__detail--font",
      font2: "question__detail--font2",
      icon: "question__content--button-icon",
      icon2: "question__content--button-icon2",
      wrapper: "question__detail--wrapper",
      wrapper2: "question__detail--wrapper2",
      button: "question__content--button",
      button2: "question__content--button2",
      height: "max-height: 0px;",
      height2: "max-height: 100%;",
    };
  },
  methods: {
    changeStatus0() {
      this.isAnswer0 = !this.isAnswer0;
    },
    changeStatus1() {
      this.isAnswer1 = !this.isAnswer1;
    },
    changeStatus2() {
      this.isAnswer2 = !this.isAnswer2;
    },
    changeStatus3() {
      this.isAnswer3 = !this.isAnswer3;
    },
  },
};
</script>

<style>
#questions {
  margin-top: 200px;
}
.question__detail--wrapper2 {
  width: 100%;
  height: 4vw;
  border-style: solid;
  border-width: thin;
  outline: none;
  background-image: linear-gradient(90deg, #fc4c3f, #ff796a);
  border-radius: 3vw;
  position: relative;
  border-color: #cecccc;
  cursor: pointer;
}

.question__content--button2 {
  width: 2vw;
  height: 2vw;
  margin-right: 1vw;
  border-radius: 50%;
  outline: none;
  background-color: #fff;
  border-color: transparent;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

.question__detail--font2 {
  font-size: 20px;
  font-family: Nunito Sans;
  margin-left: 3vw;
  margin: auto;
  margin-left: 1vw;
  font-weight: 600;
  color: #fff;
}

.question__content--button-icon2 {
  filter: invert(40%) sepia(50%) saturate(4780%) hue-rotate(340deg)
    brightness(110%) contrast(98%);
  transform: rotate(45deg);
  transition: transform 0.4s;
}

.question--wrapper {
  margin: auto;
}

.question__title--wrapper {
  display: flex;
  width: 36vw;
  margin: auto;
  justify-content: center;
  align-items: center;
}

.question__title-line--left {
  width: 5vw;
  height: 3px;
  background-image: linear-gradient(90deg, #fff, #79dcf2, #4285f4);
}

.question__title-line--right {
  width: 5vw;
  height: 3px;
  background-image: linear-gradient(90deg, #4285f4, #79dcf2, #fff);
}

.question__title--font {
  color: #0b66bf;
  font-size: 35px !important;
  font-weight: 800;
  text-align: center;
  width: auto;
  margin: auto;
  
}

.question__content--wrapper {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
  height: auto;
  justify-content: center;
  margin-top: 30px;
}

.question__item--wrapper {
  width: 43%;
  padding: 1vw;
  font-size: 20px;
}

.question__detail--wrapper {
  width: 100%;
  height: 4vw;
  border-style: solid;
  outline: none;
  background-color: transparent;
  border-width: thin;
  border-radius: 3vw;
  position: relative;
  border-color: #cecccc;
  cursor: pointer;
}

.question__detail--wrapper:hover {
  box-shadow: 3px 3px 6px #79a8f3;
}

.question__detail {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  display: flex;
  margin: auto;
  width: 100%;
  align-items: center;
  justify-content: center;
}

.question__detail--font {
  font-size: 20px;
  font-family: Nunito Sans;
  margin-left: 3vw;
  color: #202d51;
  margin: auto;
  margin-left: 1vw;
  font-weight: 600;
}

.question__content--button {
  width: 2vw;
  height: 2vw;
  margin-right: 1vw;
  border-radius: 50%;
  outline: none;
  background-image: linear-gradient(90deg, #fc4c3f, #ff796a);
  border-color: transparent;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

.question__content--button-icon {
  color: #fff;
  transition: transform 0.4s;
}

.question__answer--wrapper {
  display: flex;
  width: 100%;
  height: auto;
  margin: 0;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.4s;
}

.question__answer--detail {
  width: 100%;
  color: #626262;
  margin-top: 1vw;
  border-left-style: solid;
  border-width: thin;
  border-left-color: #cecccc;
  padding: 3px;
  margin-left: 10px;
}
</style>
