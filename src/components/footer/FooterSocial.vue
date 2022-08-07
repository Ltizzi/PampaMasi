<template lang="">
  <ul class="footer__social-ul">
    <li class="footer__social-icon" v-for="soc in social" :key="soc">
      <i :class="soc.icon"></i>
    </li>
  </ul>
</template>
<script>
  export default {
    inject: ["color", "font"],
    data() {
      return {
        social: [
          { icon: "fa-brands fa-facebook-square" },
          { icon: "fa-brands fa-instagram-square" },
        ],
      };
    },
  };
</script>
<style scoped>
  .footer__social-ul {
    display: flex;
    flex-direction: row;
    justify-content: center;
    text-align: center;
    list-style-type: none;
  }

  .footer__social-icon {
    color: v-bind("color.white");
    font-size: 5rem;
  }
</style>
