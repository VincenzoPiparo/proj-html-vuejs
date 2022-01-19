<template>
  <main>
    <div class="my_container">
      <!-- SECTION BANNER -->
      <div class="banner">
        <div class="text">
          <h1>The biggest platform for your growth.</h1>
          <p>
            There are many variations of passages of Lorem Ipsum available, but
            the majority have suffured alteration in some form
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
      <Analysis />
      <Features />
      <Cards :type="cardsArray" />
      <Testimonials />
      <Post />
      <Contact />
      <Footer :type="footerArray" />
    </div>
  </main>
</template>

<script>
import Marketing from "./Marketing.vue";
import Analysis from "./Analysis.vue";
import Features from "./Features.vue";
import Cards from "./Cards.vue";
import Testimonials from "./Testimonials.vue";
import Post from "./Post.vue";
import Contact from "./Contact.vue";
import Footer from "./Footer.vue";
export default {
  name: "Main",
  components: {
    Marketing,
    Analysis,
    Features,
    Cards,
    Footer,
    Testimonials,
    Post,
    Contact,
  },
  data: function () {
    return {
      cardsArray: [
        {
          text: "Customized Invoices",
          current: true,
        },
        {
          text: "Stock Management",
          current: false,
        },
        {
          text: "Receivable & Payables",
          current: false,
        },
        {
          text: "Manage Buying",
          current: false,
        },
        {
          text: "Powerful & Secure",
          current: false,
        },
        {
          text: "Fastest Return Filing",
          current: false,
        },
        {
          text: "Monthly Detailed",
          current: false,
        },
        {
          text: "Product Management",
          current: false,
        },
      ],
      footerArray: [
        {
          title: "Menu",
          current: true,
          text: "About Us",
          text1: "Theme",
          text2: "Features",
          text3: "Pricing",
          text4: "Blog",
        },
        {
          title: "About US",
          current: true,
          text: "About Sofbox",
          text1: "Roadmap",
          text2: "How it Work",
          text3: "Team",
          text4: "News",
        },
        {
          title: "Quick Links",
          current: true,
          text: "About Us",
          text1: "Theme",
          text2: "Features",
          text3: "Pricing",
          text4: "Blog",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../styles/variables";
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
      p {
        color: $prymary_color;
      }
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