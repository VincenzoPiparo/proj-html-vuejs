<template>
  <section>
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
.container {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}
</style>