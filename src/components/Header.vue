<template>
  <header>
    <div class="container">
      <div class="d-flex justify-content-center">
        <div class="logo mx-5 col-3">
          <img src="../assets/img/logo-2.png" alt="" />
        </div>
        <div class="navbar col-9">
          <!-- We cycle through the navigation bar each time the page is opened -->
          <div
            :class="element.current ? 'current' : null"
            v-for="(element, index) in type"
            :key="index"
          >
            {{ element.text }}
          </div>
          <!-- FONTAWESOME ICONS -->
          <div>
            <i class="fas fa-search px-5"></i>
            <i class="fas fa-shopping-cart"></i>
          </div>
          <!-- BUTTON HEADER -->
          <button type="button" class="btn btn-primary">Get Started</button>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    type: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../styles/variables";
header {
  margin-top: 20px;
  width: 100%;
  img {
    width: 70px;
  }
  .current {
    // CAMBIARE IL COLORE IN BLUE
    color: blue;
  }
}
</style>