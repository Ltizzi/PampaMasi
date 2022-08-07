<template lang="">
  <div class="home__carousel">
    <div
      id="carouselExampleCaptions"
      class="carousel slide"
      data-bs-ride="false"
    >
      <div class="carousel-indicators">
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="0"
          class="active"
          aria-current="true"
          aria-label="Slide 1"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="1"
          aria-label="Slide 2"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="2"
          aria-label="Slide 3"
        ></button>
      </div>
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img
            src="../../assets/pampa-masi/jardin.jpeg"
            class="home__img"
            alt="..."
          />
          <div class="carousel-caption d-none d-md-block">
            <h5>First slide label</h5>
            <p>Some representative placeholder content for the first slide.</p>
          </div>
        </div>
        <div class="carousel-item">
          <img
            src="../../assets/arte/talleres-de-iniciacion-artistica-y-artesanal-y-mosaiquismo/IMG_20210322_164211970.jpg"
            class="d-block w-100"
            alt="..."
          />
          <div class="carousel-caption d-none d-md-block">
            <h5>Second slide label</h5>
            <p>Some representative placeholder content for the second slide.</p>
          </div>
        </div>
        <div class="carousel-item">
          <img
            src="../../assets/entrenamiento/defensa-transfeminista/Screenshot_20220710-114114.jpg"
            class="d-block w-100"
            alt="..."
          />
          <div class="carousel-caption d-none d-md-block">
            <h5>Third slide label</h5>
            <p>Some representative placeholder content for the third slide.</p>
          </div>
        </div>
      </div>
      <button
        class="carousel-control-prev"
        type="button"
        data-bs-target="#carouselExampleCaptions"
        data-bs-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button
        class="carousel-control-next"
        type="button"
        data-bs-target="#carouselExampleCaptions"
        data-bs-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
  </div>
</template>
<script>
  export default {
    inject: ["color", "font"],
  };
</script>
<style scoped>
  .carousel {
    width: 100%;
    margin: 0 auto;
    background: v-bind("color.lightGreen");
    z-index: 0;

    /* background: var(--dark-green);
    box-shadow: 5px 5px 10px var(--toast); */
  }

  .carousel-caption {
    font-family: v-bind("font.belleza");
    font-size: 2rem;
    background: rgb(50, 50, 50, 0.5);
    width: 50%;
    margin: 0 auto;
  }

  .carousel-item {
    margin: 0 auto;
  }

  .home__img {
    width: 90%;
    height: 60vh;
    object-fit: cover;
    position: relative;
    margin-left: 7rem;
  }
</style>
