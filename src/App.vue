<template lang="">
  <the-navbar></the-navbar>
  <the-home></the-home>
  <the-footer></the-footer>
</template>
<script>
  import TheNavbar from "./components/layout/TheNavbar.vue";
  import TheHome from "./components/layout/TheHome.vue";
  import TheFooter from "./components/layout/TheFooter.vue";
  export default {
    components: {
      TheNavbar,
      TheHome,
      TheFooter,
    },
    data() {
      return {
        color: {
          toast: "#818780",
          white: "#fbfffa",
          lightGreen: "#ddf9d6",
          gray: "#e4eae4",
          green: "#76d9ad",
          darkGreen: "#67bc96",
          cyan: "#41d7df",
          blue: "#2ab4f8",
          blueToGreen: "linear-gradient(to left, #2ab4f8, #76d9ad)",
          blueToGreenVertical: "linear-gradient(to bottom, #2ab4f8, #76d9ad)",
        },

        font: {
          barrio: '"Barrio", cursive',
          arquitect: '"Architects Daughter", cursive',
          belleza: '"Belleza", sans-serif',
        },
      };
    },
    provide() {
      return {
        color: this.color,
        font: this.font,
      };
    },
  };
</script>
<style>
  * {
    margin: 0;
    padding: 0;
  }
  html {
    caret-color: transparent;
    background: v-bind("color.white");
  }
</style>
