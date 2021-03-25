<template>
  <div>
    <button
      class="btn--common btn--navbar btn--navbar--slide"
      ripple="ripple"
      @click="showPanel"
    >
      Try uniGO <em class="fas fa-download" style="padding-left: 12px"></em>
    </button>
  </div>
</template>

<script>
export default {
  name: "Nav-btn",
  methods: {
    showPanel() {
      setTimeout(() => {
        this.$emit("show_panel");
      }, 500);
    },
  },
};
</script>

<style>
@import url("../../../assets/home/common.css");
@import url("../../../assets/home/animation/Nav-btn.css");

.btn--navbar {
  height: 50px;
  width: 144px;
  box-sizing: border-box;
  background-color: white;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>