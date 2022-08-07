<template lang="">
  <div class="home">
    <home-banner></home-banner>
    <base-separador :type="true"></base-separador>
    <home-carousel></home-carousel>
    <base-separador :type="true"></base-separador>
    <div class="home__bajada">
      <h1 class="home__subtitle">
        Espacio Integral de talleres de Arte, Artesanías, Técnicas de danza,
        Entrenamiento, Consciencia corporal y actividades para Encontrarnos y
        Encontrarte
      </h1>
      <base-separador :type="true"></base-separador>
    </div>
    <home-talleres></home-talleres>
  </div>
</template>
<script>
  import HomeBanner from "../home/HomeBanner.vue";
  import HomeCarousel from "../home/HomeCarousel.vue";
  import HomeTalleres from "../home/HomeTalleres.vue";

  export default {
    inject: ["color", "font"],
    components: {
      HomeBanner,

      HomeCarousel,
      HomeTalleres,
    },
  };
</script>
<style scoped>
  .home {
    background: v-bind("color.white");
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .home__bajada {
    text-align: center;
  }

  .home__subtitle {
    text-shadow: 1px 1px 2px v-bind("color.toast");
    margin: 5rem 20rem;
    font-family: v-bind("font.arquitect");
    font-size: 3rem;
  }
</style>
