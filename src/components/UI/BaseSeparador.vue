<template lang="">
  <div class="banner" v-if="type"></div>
  <div class="footer__banner" v-if="!type"></div>
</template>
<script>
  export default {
    props: ["type"],
  };
</script>
<style scoped>
  .banner {
    padding: 1rem;
    margin: 2rem 5rem;
    background-image: url("../../assets/banner.jpeg");
    background-attachment: fixed;
    background-position: center;
    background-repeat: repeat;
    background-size: contain;
    border-radius: 10px;
  }

  .banner2 {
    padding: 2rem;
    margin: 2rem 5rem;
    background-image: url("../../assets/banner2.png");
    background-attachment: fixed;
    background-position: center;
    background-repeat: repeat;
    background-size: contain;
    border-radius: 20px;
  }

  .footer__banner {
    padding: 4rem;
    background-image: url("../../assets/banner2.png");
    background-attachment: fixed;
    background-position: center;
    background-repeat: repeat;
    background-size: contain;
    border-radius: 20px;
  }
</style>
