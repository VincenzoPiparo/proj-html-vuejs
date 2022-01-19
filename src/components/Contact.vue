<template>
  <section>
    <div class="container d-flex justify-content-center my_container">
      <h4>Contact with our team</h4>
    </div>
    <p class="d-flex justify-content-center color">
      If you are planning on developing a product landing.
    </p>

    <div class="d-flex column">
      <div class="col-6">
        <div class="street">
          <img src="../assets/img/StaticMapService.GetMapIma.png" alt="" />
        </div>
      </div>

      <div class="col-6">
        <div class="ciao flex-column bd-highlight mb-3">
          <img src="../assets/img/35.png" alt="" />

          <p class="mt-3 bold">9840 Shore St.Fond Du Lac, WI 54935</p>
          <p class="color">0 1223 456 789</p>
          <p class="color">mail@example.com</p>

          <div class="icons">
            <i class="fab fa-facebook-f"></i>
            <i class="fab fa-twitter"></i>
            <i class="fab fa-github"></i>
            <i class="fab fa-instagram"></i>
          </div>

          <h4>Get in Touch</h4>
          <!-- INPUT NAME -->
          <div class="input-group mb-3 my_input">
            <div class="input-group-prepend"></div>
            <input
              type="text"
              class="form-control"
              placeholder="Your Name"
              aria-label="Your Name"
              aria-describedby="basic-addon1"
            />
          </div>
          <!-- INPUT EMAIL -->

          <div class="input-group mb-3 my_input">
            <div class="input-group-prepend"></div>
            <input
              type="text"
              class="form-control"
              placeholder="Your Name"
              aria-label="Your Name"
              aria-describedby="basic-addon1"
            />
          </div>

          <!-- INPUT SUBJECT -->
          <div class="input-group mb-3">
            <div class="input-group-prepend"></div>
            <input
              type="text"
              class="form-control"
              placeholder="Your Subject"
              aria-label="Your Subject"
              aria-describedby="basic-addon1"
            />
          </div>

          <!-- INPUT TEXT AREA -->
          <div class="input-group message">
            <textarea
              class="form-control"
              placeholder="Your Message"
              aria-label="With textarea"
            ></textarea>
          </div>

          <!-- BUTTON -->
          <button type="button" class="btn btn-primary mt-5">
            Send Message
          </button>
        </div>
      </div>
    </div>
  </section>
</template>


<style lang="scss" scoped>
@import "../styles/variables";
.my_container {
  margin-top: 150px;
  .bold {
    font-weight: bold;
  }
  .color {
    color: $prymary_color;
  }
  .column {
    margin-top: 80px;
    .icons {
      i {
        margin: 0 10px;
        border: 1px solid lightgray;
        border-radius: 5px;
        padding: 5px 10px;
        height: 30px;
        color: #377dff;
      }
    }
    h4 {
      margin-top: 25px;
    }
  }
  .my_input {
    width: 250px;
  }
  .message {
    height: 150px;
  }
}
</style>