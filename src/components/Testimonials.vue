<template>
  <section>
    <div class="container">
      <div class="d-flex justify-content-center">
        <h4>Our Testimonials</h4>
      </div>
      <p class="d-flex justify-content-center">
        If you are planning on developing a product landing app or website, take
        a look at this beautiful-crafted
      </p>
      <div class="box-container d-flex justify-content-between">
        <!-- BOX SHADOW -->
        <div class="box-shadow shadow-lg p-3 mb-5 bg-white rounded"></div>
        <div class="box-behind shadow-lg p-3 mb-5 bg-white rounded"></div>
        <!-- BOX 1 -->
        <div
          class="
            box-image
            shadow-lg
            p-3
            mb-5
            bg-white
            rounded
            d-flex
            align-items-center
            flex-column
          "
        >
          <div class="d-flex justify-content-center">
            <img class="w-50" src="../assets/img/26.jpeg" alt="" />
          </div>
          <h4 class="text-center mt-5 w-100">
            Julia <span>- COO Sofbox</span>
          </h4>
          <p class="px-5 mt-5">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
            molestias veniam ducimus dolorum nemo cum ipsa, incidunt tempora
            deleniti doloribus provident amet dicta iure aspernatur, laudantium
            saepe reprehenderit ullam neque.
          </p>
        </div>
        <!-- BOX 2 -->
        <div
          class="
            box-image
            shadow-lg
            p-3
            mb-5
            bg-white
            rounded
            d-flex
            align-items-center
            flex-column
          "
        >
          <div class="d-flex justify-content-center">
            <img class="w-50" src="../assets/img/27.jpeg" alt="" />
          </div>

          <h4 class="text-center mt-5 w-100">
            Julia <span>- COO Sofbox</span>
          </h4>
          <p class="px-5 mt-5">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
            molestias veniam ducimus dolorum nemo cum ipsa, incidunt tempora
            deleniti doloribus provident amet dicta iure aspernatur, laudantium
            saepe reprehenderit ullam neque.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import "../styles/variables";
.container {
  .box-behind {
    position: absolute;
    width: 350px;
    height: 445px;

    left: 370px;
  }
  .box-shadow {
    position: absolute;
    width: 400px;
    height: 420px;

    left: 350px;
    z-index: 5;
  }
  .box-image {
    z-index: 10;
    width: 500px;
    height: 400px;

    border-radius: 10px;
    img {
      margin-top: 30px;
      width: 100%;
    }
    span {
      color: $prymary_color;
    }
  }
  p {
    color: $prymary_color;
  }
  margin-top: 200px;
}
</style>