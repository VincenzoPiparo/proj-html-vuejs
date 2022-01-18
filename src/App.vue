<template>
  <div id="app">
    <Header :type="navArray" />
    <Main />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
export default {
  name: "App",
  components: {
    Header,
    Main,
  },
  data: function () {
    return {
      navArray: [
        {
          text: "Home",
          current: true,
        },
        {
          text: "About us",
          current: false,
        },
        {
          text: "Feature",
          current: false,
        },
        {
          text: "Testimonials",
          current: false,
        },
        {
          text: "Contact US",
          current: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./styles/general";
@import "../node_modules/bootstrap";
</style>
