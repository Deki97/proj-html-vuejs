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
          reference: '+1 (305) 1234-5678'
        },
        {
          reference: 'hello@example.com'
        },
        {
          reference: 'Main Avenue, 987'
        }
      ]
    }
  }
};
</script>


<style lang="scss">
@import './style/general.scss';

</style>
