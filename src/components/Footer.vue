<template>
  <!-- Footer -->

  <footer class="text-center text-lg-start text-muted mt-5">
    <!-- Section: Social media -->
    <section
      class="
        d-flex
        justify-content-center justify-content-lg-between
        p-4
        border-bottom
      "
    ></section>
    <!-- Section: Social media -->

    <!-- Section: Links  -->
    <section>
      <div class="container text-center text-md-start mt-5">
        <!-- Grid row -->
        <div class="row mt-3">
          <!-- Grid column -->
          <div class="col-md-3 col-lg-4 col-xl-3 mx-auto mb-4">
            <!-- Content -->

            <img src="../assets/img/35.png" alt="sofbox" />

            <p class="color">
              Here you can use rows and columns to organize your footer content.
              Lorem ipsum dolor sit amet, consectetur adipisicing elit.
            </p>

            <div>Copyright @ 2018 <span class="copyright">Sofbox</span></div>
          </div>
          <!-- Grid column -->

          <!-- Grid column -->

          <div
            :class="element.current ? 'current' : null"
            v-for="(element, index) in type"
            :key="index"
            class="col-md-2 col-lg-2 col-xl-2 mx-auto mb-4"
          >
            <!-- Links -->
            <h6 class="text-uppercase fw-bold mb-4">{{ element.title }}</h6>
            <p class="color">
              <a href="#" class="text-reset">{{ element.text }}</a>
            </p>
            <p class="color">
              <a href="#" class="text-reset">{{ element.text1 }}</a>
            </p>
            <p class="color">
              <a href="#" class="text-reset">{{ element.text2 }}</a>
            </p>
            <p class="color">
              <a href="#" class="text-reset">{{ element.text3 }}</a>
            </p>
            <p class="color">
              <a href="#" class="text-reset">{{ element.text4 }}</a>
            </p>
          </div>
        </div>
        <!-- Grid column -->

        <!-- Grid row -->
      </div>
    </section>
    <!-- Section: Links  -->
  </footer>
  <!-- Footer -->
</template>

<script>
export default {
  name: "Footer",
  props: {
    type: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../styles/variables";
section {
  .copyright {
    font-weight: bold;
    color: #377dff;
  }
  .color {
    color: $prymary_color;
    a {
      text-decoration: none;
    }
  }
}
</style>