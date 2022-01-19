<template>
  <div id="app">
    <Header :stringMenu="header_menus" />

    <Main />

    <Footer />
  </div>
</template>


<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer
  },
  data: function() {
    return {
      header_menus: [
        {
          tab: 'Home'
        },
        {
          tab: 'About'
        },
        {
          tab: 'Projects'
        },
        {
          tab: 'Process'
        },
        {
          tab: 'Testimonials'
        }
      ]
    }
  }
};
</script>


<style lang="scss">
@import './style/general.scss';

</style>
