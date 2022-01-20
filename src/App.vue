<template>
  <div id="app">
    <!-- Passo tramite delle props l'array di stringhe menu al componente Header -->
    <Header :objectMenu="header_menus" />

    <Main />

    <!-- Passo tramite delle props l'array di stringhe menu al componente footer -->
    <Footer :objectText="footer_menus" />
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
      // Array di oggetti dove ogni stringa rappresenta un menu dell'header
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
      // Array di oggetti dove ogni stringa rappresenta un paragrafo del footer
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
