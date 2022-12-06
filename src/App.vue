<template>
  <div id="app">
    <HeaderComp :nav="nav" />
    <JumbotronComp />
    <MainComp :latest_post="latest_post" :key_features="key_features" :testimonials="testimonials" />
    <FooterComp :footer="footer" />
  </div>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue";
import JumbotronComp from "./components/JumbotronComp.vue";
import MainComp from "./components/MainComp.vue";
import FooterComp from "./components/FooterComp.vue";

export default {
  name: "App",
  components: {
    HeaderComp,
    JumbotronComp,
    MainComp,
    FooterComp,
  },
  data() {
    return {
      nav: [
        {
          id: 1,
          name: "Home",
        },
        {
          id: 2,
          name: "About us",
        },
        {
          id: 3,
          name: "Feature",
        },
        {
          id: 4,
          name: "Testimonials",
        },
        {
          id: 5,
          name: "Contact US",
        },
      ],

      testimonials: [
        {
          id: 1,
          photo: "26.jpeg",
          name: "Julia",
          firstname: "Aann",
          role: "COO Softbox",
          description:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.",
        },
        {
          id: 2,
          photo: "27.jpeg",
          name: "Mac",
          firstname: "Znder",
          role: "Manager Sofbox",
          description:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.",
        },
      ],
      footer: [
        {
          id: 1,
          name: "Menu",
          options_menu: [
            {
              id: 1,
              name: "About us",
            },
            {
              id: 2,
              name: "Theme",
            },
            {
              id: 3,
              name: "Features",
            },
            {
              id: 4,
              name: "Pricing",
            },
            {
              id: 5,
              name: "Blog",
            },
          ],
        },
        {
          id: 2,
          name: "About Us",
          options_menu: [
            {
              id: 1,
              name: "About Solfbox",
            },
            {
              id: 2,
              name: "Roadmap",
            },
            {
              id: 3,
              name: "How it Work",
            },
            {
              id: 4,
              name: "Team",
            },
            {
              id: 5,
              name: "News",
            },
          ],
        },
        {
          id: 3,
          name: "Quick Links",
          options_menu: [
            {
              id: 1,
              name: "About us",
            },
            {
              id: 2,
              name: "Theme",
            },
            {
              id: 3,
              name: "Features",
            },
            {
              id: 4,
              name: "Pricing",
            },
            {
              id: 5,
              name: "Blog",
            },
          ],
        },
      ],

      latest_post: [
        {
          id: 1,
          img: "19.jpg",
          data: "November 28. 2019",
          title: "Life Lack Meaning",
          description:
            "it is a long estabilished fact that a reader will be distracted by the readable.",
        },
        {
          id: 2,
          img: "18.jpg",
          data: "November 28. 2019",
          title: "Life Lack Meaning",
          description:
            "it is a long estabilished fact that a reader will be distracted by the readable.",
        },
        {
          id: 3,
          img: "17.jpg",
          data: "November 28. 2019",
          title: "Life Lack Meaning",
          description:
            "it is a long estabilished fact that a reader will be distracted by the readable.",
        },
      ],

      key_features: [
        {
          id: 1,
          name: "Customized Invoices",
          img: "customized.png",
        },
        {
          id: 2,
          name: "Stock Management",
          img: "stock.png",
        },
        {
          id: 3,
          name: "Receivable & Payables",
          img: "receivable.png",
        },
        {
          id: 4,
          name: "Manage Buying",
          img: "manage.png",
        },
        {
          id: 5,
          name: "Powerful & Secure",
          img: "powerful.png",
        },
        {
          id: 6,
          name: "Fastest Return Filing",
          img: "receivable.png",
        },
        {
          id: 7,
          name: "Monthly Detailed",
          img: "Monthly.png",
        },
        {
          id: 8,
          name: "Product Management",
          img: "product.png",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Comfortaa", cursive;
}

.conteiner-sito{
  width: 70%;
  margin: 0 auto
}

@import url("https://fonts.googleapis.com/css2?family=Comfortaa&family=Heebo&family=Inter&family=Kanit:ital@1&family=Noto+Sans&family=PT+Sans:ital@1&family=Roboto&family=Ubuntu&display=swap");
</style>
