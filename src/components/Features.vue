<template>
  <section id="features">
    <div class="features--wrapper">
      <div class="features--content">
        <div class="features__title--wrapper">
          <div class="features__title--font">
            <h1>What does uniGO offer?</h1>
            <div class="feature__title-line--separator"></div>
          </div>
          <div class="features__title--description">
            Being a technology-based solution developed on mobile app, uniGO
            offers the following features:
          </div>
        </div>
        <div class="features">
          <div
            data-aos="fade-right"
            data-aos-duration="2000"
            class="info_1 aos-init aos-animate"
          >
            <div class="info_1--title">
              <img
                src="../assets/number 1.svg"
                class="info_1--img"
                alt="number 1"
              />
              <div style="margin-left: 1%; color: rgb(98, 98, 98)">
                <h3>Location Information</h3>
                <p class="features__title--description">
                  Allowing users to look up details about locations in the
                  University and locate current position using QR code or GPS…
                </p>
              </div>
            </div>
          </div>
          <div
            data-aos="zoom-in-left"
            data-aos-duration="1500"
            class="pic1-bg aos-init aos-animate"
          >
            <img src="../assets/qrcode-01 1.svg" class="pic1" />
          </div>
          <div
            data-aos="zoom-in"
            data-aos-duration="2000"
            class="pic2-bg aos-init aos-animate"
          >
            <img src="../assets/Pic.svg" class="pic2" />
          </div>
          <div
            data-aos="fade-left"
            data-aos-duration="2000"
            class="info_2 aos-init aos-animate"
          >
            <div class="info_2--title">
              <img src="../assets/number 2.svg" class="info_2--img" />
              <div style="margin-left: 1%; color: rgb(98, 98, 98)">
                <h3>Route Planning</h3>
                <p class="features__title--description">
                  Directions Feature helps identify the shortest path to your
                  destinations.
                </p>
              </div>
            </div>
          </div>

          <div
            data-aos="fade-right"
            data-aos-duration="1500"
            class="info_1 aos-init aos-animate"
            id="features__room-info--text"
          >
            <div class="info_1--title" id="features__room-info--text">
              <img src="../assets/number 3 1.svg" class="info_1--img" />
              <div style="margin-left: 1%; color: rgb(98, 98, 98)">
                <h3>Classroom Information</h3>
                <p class="features__title--description">
                  By installing uniGO, users will be able to search for
                  information on classrooms, lecturers and credit classes at a
                  specific time.
                </p>
              </div>
            </div>
          </div>
          <div
            data-aos="zoom-in"
            data-aos-duration="2000"
            class="pic1-bg search aos-init aos-animate"
          >
            <img src="../assets/3-01 1.svg" class="pic1" />
          </div>

          <div
            data-aos="zoom-in"
            data-aos-duration="1500"
            class="pic2-bg announcement aos-init aos-animate"
          >
            <img src="../assets/tb-01 1.svg" class="pic2" />
          </div>
          <div
            data-aos="fade-left"
            data-aos-duration="2000"
            class="info_2 aos-init aos-animate"
            id="features__school-event--text"
          >
            <div class="info_2--title">
              <img src="../assets/number 4.svg" class="info_2--img" />
              <div style="margin-left: 1%; color: rgb(98, 98, 98)">
                <h3>Events Notifying</h3>
                <p class="features__title--description">
                  uniGO keeps undergraduates informed about events hosted by the
                  University, Clubs and Organizations.
                </p>
              </div>
            </div>
          </div>
          <div id="users"><div></div></div>
        </div>
      </div>
      <div class="button-up">
        <div style="position: relative; height: 7vw">
          <a href="#home"
            ><div id="footer--button" class="footer--button">
              <img
                src="../assets/arrow-down-sign-to-navigate 1.svg"
                class="footer--button-img"
              /></div
          ></a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Features",
};
</script>

<style>
#features {
  margin-top: 100px;
}
#features__school-event--text {
  top: 90vw;
}
#features__room-info--text {
  top: 60vw;
}
.announcement {
  top: 80vw !important;
  left: 20% !important;
}
.search {
  top: 49vw !important;
  left: 57% !important;
}
.button-up {
  position: fixed;
  right: 0;
  top: 85%;
  z-index: 1000;
}
.features--content {
  width: 100%;
}
.features {
  position: relative;
  padding: 10px;
  font-family: Nunito Sans;
  width: auto;
  height: 100vw;
  background-image: url("../assets/line-01\ 1.svg");
  background-size: 100% 100%;
}
.line-bg {
  width: auto;
  height: 100%;
  position: absolute;
  top: 10vw;
  left: 50%;
  transform: translateX(-50%);
}
.line {
  width: auto;
  transform: rotate(0.8deg);
}
.pic1-bg {
  position: absolute;
  top: -8vw;
  left: 62%;
}
.pic1 {
  width: 25vw;
  height: 25vw;
}
.pic2-bg {
  position: absolute;
  top: 23vw;
  left: 16%;
}
.pic2 {
  width: 24vw;
  height: 24vw;
}
.info_1 {
  position: absolute;
  top: 0;
  left: 20%;
  font-size: 18px;
  width: 28vw;
}
.info_1--title {
  display: flex;
  align-items: flex-start;
}
.info_1--img {
  width: 10%;
  height: auto;
}
.info_2 {
  position: absolute;
  top: 30vw;
  right: 20%;
  font-size: 18px;
  width: 28vw;
}
.info_2--title {
  display: flex;
  align-items: flex-start;
}
.info_2--img {
  width: 10%;
  height: auto;
}
.features h3 {
  color: #202d51;
  font-size: 25px !important;
  font-weight: 700;
  line-height: 3vw;
}
.features--wrapper {
  padding: 12px;
}
.features__title--wrapper {
  width: 40%;
  height: 15vw;
  margin-left: 110px;
}
.features__title--font {
  display: flex;
  height: 30%;
  align-items: center;
}
.features__title--font h1 {
  font-size: 35px;
  font-weight: 800;
  color: #0b66bf;
  margin: 0;
}
.features__title--description {
  font-size: 20px;
  line-height: 27px;
  color: #626262;
}
.feature__title-line--separator {
  margin-top: 8px;
  margin-left: 20px;
  width: 10vw;
  height: 4px;
  background-image: linear-gradient(
    90deg,
    #4285f4 -19.99%,
    rgba(121, 220, 242, 0) 94.51%
  );
}
</style>

