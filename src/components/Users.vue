<template>
  <section id="user">
    <div class="users">
      <div class="users__title">
        <div class="users__title--font">Targeted Users</div>
      </div>

      <!-- Students -->
      <div
        data-aos="zoom-in"
        data-aos-duration="1500"
        class="users__students-line--wrapper"
      >
        <img class="users__students--line" src="../assets/line.svg" />
      </div>
      <div class="users__students--wrapper students">
        <div
          data-aos="zoom-in"
          data-aos-duration="1500"
          class="users__img--shadow"
          style="position: relative"
        >
          <img
            class="users__students--image"
            src="../assets/Sinh vien (1).svg"
          />
          <div class="users__img--circle"></div>
        </div>
        <div
          data-aos="zoom-in"
          data-aos-duration="1500"
          class="users__contents--wrapper"
        >
          <h2>Undergraduates</h2>
          <p v-if="isShort0" class="users__students--description-summary">
            With uniGO, undergraduates can search for classroom information...
          </p>
          <p v-if="!isShort0" class="users__students--description-summary">
            With uniGO, undergraduates can search for classroom information and
            receive personal notifications for their credit courses.
          </p>
          <button
            @click="isShort0 = !isShort0"
            v-if="isShort0"
            class="users__students--description-full"
          >
            Learn more
          </button>
        </div>
      </div>
      <!-- End Students -->

      <!-- Freshman -->
      <div
        data-aos="zoom-in"
        data-aos-duration="1500"
        class="users__freshman-line--wrapper"
      >
        <img class="users__freshman--line" src="../assets/line (1).svg" />
      </div>
      <div class="users__students--wrapper freshman--content">
        <div
          data-aos="zoom-in"
          data-aos-duration="1500"
          class="users__img--shadow"
          style="position: relative"
        >
          <img
            class="users__students--image freshman--img"
            src="../assets/TSV-01.svg"
          />
          <div class="users__img--circle"></div>
        </div>
        <div
          data-aos="zoom-in"
          data-aos-duration="1500"
          class="users__contents--wrapper"
        >
          <h2>Freshmen</h2>
          <p v-if="isShort1" class="users__students--description-summary">
            uniGO is a “life-saver” that makes it easier for newbies to find...
          </p>
          <p v-if="!isShort1" class="users__students--description-summary">
            uniGO is a “life-saver” that makes it easier for newbies to find
            lecture halls as well as information and location of functional
            departments.
          </p>
          <button
            @click="isShort1 = !isShort1"
            v-if="isShort1"
            class="users__students--description-full"
          >
            Learn more
          </button>
        </div>
      </div>
      <!-- End Freshman -->

      <!-- Lecturers -->
      <div
        data-aos="zoom-in"
        data-aos-duration="1500"
        class="users__lecturers-line--wrapper"
      >
        <img class="users__lecturers--line" src="../assets/line (2).svg" />
      </div>
      <div class="users__students--wrapper lecturers--content">
        <div
          data-aos="zoom-in"
          data-aos-duration="1500"
          class="users__img--shadow"
          style="position: relative"
        >
          <img
            class="users__students--image lecturers--img"
            src="../assets/GV-01.svg"
          />
          <div class="users__img--circle"></div>
        </div>
        <div
          data-aos="zoom-in"
          data-aos-duration="1500"
          class="users__contents--wrapper lecturers-width"
        >
          <h2>Lecturers</h2>
          <p v-if="isShort2" class="users__students--description-summary">
            uniGO assists lecturers in managing their teaching schedule...
          </p>
          <p v-if="!isShort2" class="users__students--description-summary">
            uniGO assists lecturers in managing their teaching schedule and
            receiving related notices.
          </p>
          <button
            @click="isShort2 = !isShort2"
            v-if="isShort2"
            class="users__students--description-full"
          >
            Learn more
          </button>
        </div>
      </div>
      <!-- End Lecturers -->

      <!-- Guests -->
      <div
        data-aos="zoom-in"
        data-aos-duration="1500"
        class="users__guests-line--wrapper"
      >
        <img class="users__guests--line" src="../assets/Group (1).svg" />
      </div>
      <div class="users__students--wrapper guests--content">
        <div
          data-aos="zoom-in"
          data-aos-duration="1500"
          class="users__img--shadow"
          style="position: relative; background-color: transparent"
        >
          <img
            class="users__students--image guests--img"
            src="../assets/KTQ-01.svg"
          />
          <div class="users__img--circle"></div>
        </div>
        <div
          data-aos="zoom-in"
          data-aos-duration="1500"
          class="users__contents--wrapper"
        >
          <h2>Visitors</h2>
          <p
            v-if="isShort3"
            class="users__students--description-summary summary--bot"
          >
            Without asking for help or looking at the old-fashioned map...
          </p>
          <p
            v-if="!isShort3"
            class="users__students--description-summary summary--bot"
          >
            Without asking for help or looking at the old-fashioned map, when
            visitors install uniGO, they will be able to explore the beautiful
            campus with an area of more than 24ha.F.
          </p>
          <button
            @click="isShort3 = !isShort3"
            v-if="isShort3"
            class="users__students--description-full"
          >
            Learn more
          </button>
        </div>
      </div>
      <!-- End Guests -->

      <!-- Clubs -->
      <div
        data-aos="zoom-in"
        data-aos-duration="1500"
        class="users__clubs-line--wrapper"
      >
        <img class="users__clubs--line" src="../assets/Group (3).svg" />
      </div>
      <div class="users__students--wrapper clubs-content">
        <div
          data-aos="zoom-in"
          data-aos-duration="1500"
          class="users__img--shadow"
          style="position: relative; background-color: transparent"
          id="clb--image-sm"
        >
          <img class="users__students--image" src="../assets/CLB-01.svg" />
          <div class="users__img--circle"></div>
        </div>
        <div
          data-aos="zoom-in"
          data-aos-duration="1500"
          class="users__contents--wrapper"
        >
          <h2>Clubs, Organizations</h2>
          <p
            v-if="isShort4"
            class="users__students--description-summary summary--bot"
          >
            Clubs and Organizations can suggest their guests to actively
            search...
          </p>
          <p
            v-if="!isShort4"
            class="users__students--description-summary summary--bot"
          >
            Clubs and Organizations can suggest their guests to actively search
            for revenue information using uniGO in order to make the events go
            smoothly without a hitch.
          </p>
          <button
            @click="isShort4 = !isShort4"
            v-if="isShort4"
            class="users__students--description-full"
          >
            Learn more
          </button>
        </div>
      </div>
      <!-- End Clubs -->
    </div>
  </section>
</template>

<script>
export default {
  name: "Users",
  data() {
    return {
      isShort0: true,
      isShort1: true,
      isShort2: true,
      isShort3: true,
      isShort4: true,
    };
  },
};
</script>

<style>
.users {
  margin-top: 10vw;
  display: block;
  position: relative;
  height: 38vw;
  padding: 10px;
}
.users__title {
  width: 23vw;
  height: 6vw;
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  background-color: #fc4c3f;
  border-radius: 3vw;
  z-index: 2;
}
.users__title--font {
  position: absolute;
  width: 80%;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: #fff;
  font-size: 28px;
  font-weight: 700;
}
.users__students-line--wrapper {
  position: absolute;
  top: 3vw;
  left: 20%;
}
.users__students--line {
  width: 18vw;
  height: auto;
}
.users__students--wrapper {
  position: absolute;
  top: 3vw;
  left: 12%;
}
.users__students--image {
  width: 8vw;
  height: 8vw;
  background-color: #fff;
}
.users__students--description-summary {
  color: #626262;
  font-size: 20px;
  line-height: 27px;
  width: 100%;
  height: auto;
  margin-top: 2vw;
}
.users__students--description-full {
  color: #000;
  font-size: 15px;
  text-decoration: underline;
  color: #202d51;
  margin-top: 2vw;
  background-color: transparent;
  outline: none;
  border-style: hidden;
  cursor: pointer;
  font-weight: 700;
}
.lecturers-width {
  width: 11vw !important;
}
.users__freshman-line--wrapper {
  position: absolute;
  top: 5vw;
  left: 32%;
}
.users__freshman--line {
  width: 8vw;
  height: auto;
}
.freshman--content {
  top: 12vw;
  left: 28%;
  border-color: #ff796a;
}
.users__contents--wrapper {
  width: 12vw;
  height: auto;
  color: #626262;
}
.users h2 {
  color: #202d51;
  margin-top: 10%;
  font-size: 25px;
  font-weight: 700;
}
.users__lecturers-line--wrapper {
  position: absolute;
  top: 6vw;
  left: 50%;
  transform: translateX(-50%) !important;
}
.users__lecturers--line {
  width: 1vw;
  height: auto;
}
.lecturers--content {
  top: 11vw;
  left: 52%;
  transform: translateX(-55%);
}
.users__guests-line--wrapper {
  position: absolute;
  top: 5vw;
  left: 64%;
  transform: translateX(-50%) !important;
}
.users__guests--line {
  width: 8vw;
  height: auto;
}
.guests--content {
  top: 12vw;
  left: 69%;
  transform: translateX(-50%);
  border-color: #ff796a;
}
.users__clubs-line--wrapper {
  position: absolute;
  top: 3vw;
  left: 71%;
  transform: translateX(-50%) !important;
}
.users__clubs--line {
  width: 18vw;
  height: auto;
}
.users__img--shadow {
  position: relative;
  width: 8vw;
  height: 8vw;
}
.users__img--circle {
  height: 7vw;
  width: 7vw;
  position: absolute;
  top: 49%;
  left: 51%;
  transform: translate(-50%, -50%);
  border-radius: 50%;
  box-shadow: 3px 3px 6px rgba(0, 0, 0, 0.27058823529411763);
}
.clubs-content {
  top: 3vw;
  left: 85%;
  transform: translateX(-50%);
  border-color: #0b66bf;
}
</style>