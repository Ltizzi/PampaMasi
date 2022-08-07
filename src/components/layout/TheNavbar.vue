<template lang="">
  <nav class="nav">
    <ul class="nav-bar">
      <li class="nav-item">Home</li>
    </ul>
    <ul class="nav-bar">
      <li class="nav-item">Historia</li>
      <li class="nav-item">Experiencias</li>
      <li class="nav-item">Nosotros</li>
      <li class="nav-item">Horarios</li>
      <li class="nav-item">Galeria</li>
      <li class="nav-item">Contacto</li>
    </ul>
  </nav>
</template>
<script>
  export default {
    inject: ["color", "font"],
  };
</script>
<style scoped>
  .nav {
    background: v-bind("color.blueToGreen");
    padding: 1rem 2rem;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    position: fixed;
    width: 100%;
    z-index: 1;
  }

  .nav-bar {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    color: v-bind("color.white");
    font-family: v-bind("font.arquitect");
    font-size: 1.5rem;
    text-shadow: 3px 3px 4px v-bind("color.toast");
  }

  .nav-item {
    margin-right: 2rem;
    list-style-type: none;
  }
</style>
