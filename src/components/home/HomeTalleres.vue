<template lang="">
  <div class="home__talleres">
    <div class="home__talleres-picrow">
      <img
        v-for="img in imgRowTop"
        :key="img"
        :src="require(`@/assets${img.foto}`)"
        :alt="img.text"
        class="home__talleres-pic"
      />
    </div>
    <div class="home__talleres-title">Talleres</div>
    <div class="home__talleres-picrow">
      <img
        v-for="img in imgRowBottom"
        :key="img"
        :src="require(`@/assets${img.foto}`)"
        :alt="img.text"
        class="home__talleres-pic"
      />
    </div>
  </div>
</template>
<script>
  export default {
    inject: ["color", "font"],
    data() {
      return {
        imgRowTop: [
          {
            foto: "/arte/talleres-de-iniciacion-artistica-y-artesanal-y-mosaiquismo/IMG_20210322_164211970.jpg",
            text: "Alumnos trabajando en el taller",
          },
          {
            foto: "/arte/talleres-de-iniciacion-artistica-y-artesanal-y-mosaiquismo/IMG_20220314_161619623.jpg",
            text: "Más alumnos trabajando en el taller",
          },
        ],
        imgRowBottom: [
          {
            foto: "/movimiento/baile/Screenshot_20220710-114023.jpg",
            text: "Taller de Danza",
          },
          {
            foto: "/entrenamiento/defensa-transfeminista/Screenshot_20220710-114722.jpg",
            text: "Práctica de defensa personal transfeminista",
          },
        ],
      };
    },
  };
</script>
<style scoped>
  .home__talleres {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    background: v-bind("color.blueToGreen");
    box-shadow: 5px 5px 10px v-bind("color.toast");
    border-radius: 50px;
    margin: 0 15rem;
  }

  .banner-vertical {
    padding: 0.5rem;
    background: v-bind("color.blueToGreenVertical");
  }

  .home__talleres-picrow {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
  }

  .home__talleres-pic {
    border-radius: 50%;
    width: 22rem;
    height: 22rem;
    margin: 1.5rem 0;
    box-shadow: 5px 5px 10px v-bind("color.gray");
  }

  .home__talleres-title {
    font-family: v-bind("font.belleza");
    text-align: center;
    font-size: 8rem;
    color: v-bind("color.white");
    text-shadow: 5px 5px 10px v-bind("color.toast");
    margin: -5rem 0;
  }
</style>
