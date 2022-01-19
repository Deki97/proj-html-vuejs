<template>
  <div id="app">
    <Header :stringMenu="header_menus" />

    <Main />

    <Footer :stringParagraph="footer_menus" />
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
          menu: 'Home'
        },
        {
          menu: 'About'
        },
        {
          menu: 'Projects'
        },
        {
          menu: 'Process'
        },
        {
          menu: 'Testimonials'
        },
      ],
      footer_menus: [
        {
          text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
        },
        {
          text: 'Praesent diam lacus, dapibus sed imperdiet consectetur.'
        }
      ]
    }
  }
};
</script>


<style lang="scss">
@import './style/general.scss';

</style>
