<template lang="">
  <img src="../../assets/logo-grande.png" alt="" class="home__logo" />
  <h1 class="home__title">Frase de Bienvenida</h1>
</template>
<script>
  export default {
    inject: ["color", "font"],
  };
</script>
<style scoped>
  .home__title {
    font-family: v-bind("font.belleza");
    text-align: center;
    font-size: 5rem;
    color: v-bind("color.toast");
    margin: 3rem auto;
  }

  .home__logo {
    width: 30rem;
    margin: 0 auto;
    margin-top: 10rem;
    border-radius: 50%;
    box-shadow: 10px 10px 30px 10px v-bind("color.gray");
  }
</style>
