<template>
  <div id="app">
    <HeaderComp  :nav="nav" />
    <JumbotronComp />
    <MainComp />
    <FooterComp />
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
          name: 'Home',
        },
        {
          id: 2,
          name: 'About us',
        },
        {
          id: 3,
          name: 'Feature',
        },
        {
          id: 4,
          name: 'Testimonials',
        },
        {
          id: 5,
          name: 'Contact US',
        },
      ],

      Testimonials:[
        {
          id: 1,
          photo: '26.jpeg',
          name: 'Julia',
          firstname: 'Aann',
          role: 'COO Softbox',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur'
        },
         {
          id: 2,
          photo: '27.jpeg',
          name: 'Mac',
          firstname: 'Znder',
          role: 'Manager Sofbox',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur'
        }
      ],
      footer:[
        {
          id: 1,
          name: 'Menu',
          options_menu:[
            {
              id: 1,
              name: 'About us',
            },
            {
              id: 2,
              name: 'Theme',
            },
            {
              id: 3,
              name: 'Features',
            },
            {
              id: 4,
              name: 'Pricing',
            },
            {
              id: 5,
              name: 'Blog',
            },

          ],

        },
        {
          id: 2,
          name: 'About Us',
          options_menu:[
            {
              id: 1,
              name: 'About Solfbox',
            },
            {
              id: 2,
              name: 'Roadmap',
            },
            {
              id: 3,
              name: 'How it Work',
            },
            {
              id: 4,
              name: 'Team',
            },
            {
              id: 5,
              name: 'News',
            },

          ]

        },
        {
          id: 3,
          name:'Quick Links',
          options_menu:[
            {
              id: 1,
              name: 'About us',
            },
            {
              id: 2,
              name: 'Theme',
            },
            {
              id: 3,
              name: 'Features',
            },
            {
              id: 4,
              name: 'Pricing',
            },
            {
              id: 5,
              name: 'Blog',
            },

          ]

        }

      ]
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
}
</style>
