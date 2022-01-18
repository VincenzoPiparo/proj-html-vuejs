<template>
  <main>
    <div class="my_container">
      <!-- SECTION BANNER -->
      <div class="banner">
        <div class="text">
          <h1>The biggest platform for your growth.</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo
            tempora quis similique asperiores quas harum? Molestiae veniam quam
            distinctio. Hic at cum tempora tempore id itaque maiores amet porro
            quae?
          </p>
          <button type="button" class="btn btn-primary my_btn">
            Read More
          </button>
        </div>
        <div class="logo">
          <img src="../assets/img/27-1.png" alt="" />
        </div>
      </div>
      <Marketing />
    </div>
  </main>
</template>

<script>
import Marketing from "./Marketing.vue";
export default {
  name: "Main",
  components: {
    Marketing,
  },
};
</script>

<style lang="scss" scoped>
main {
  .my_container {
    width: 80%;
    margin: auto;
    border-radius: 10px;
    background-color: #f2f7ff;
    height: 400px;
    .banner {
      margin-top: 40px;
      display: flex;
    }
    .text {
      width: 50%;
      margin-top: 50px;
      margin-left: 50px;
      display: flex;
      flex-direction: column;
      .my_btn {
        width: 150px;
      }
    }
    .logo {
      margin-top: 50px;
      margin-left: 50px;
      display: flex;
      justify-content: flex-end;
    }
  }
}
</style>