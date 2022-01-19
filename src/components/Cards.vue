<template>
  <section>
    <div class="position-relative">
      <div class="container">
        <div
          :class="element.current ? 'current' : null"
          v-for="(element, index) in type"
          :key="index"
          class="card mt-3"
          style="width: 18rem"
        >
          <div class="card-body">
            <h5 class="card-title">
              {{ element.text }}
            </h5>
          </div>
        </div>
      </div>
      <div class="background_circle">
        <img src="../assets/img/14.png" alt="circle" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Cards",
  props: {
    type: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../styles/variables";
.background_circle {
  position: absolute;
  left: -600px;
  top: -300px;
}
.container {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}
</style>