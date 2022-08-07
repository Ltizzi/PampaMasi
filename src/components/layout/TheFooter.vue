<template lang="">
  <footer class="footer">
    <base-separador :type="false"></base-separador>
    <div class="footer__social">
      <footer-social></footer-social>
    </div>
  </footer>
</template>
<script>
  import FooterSocial from "../footer/FooterSocial.vue";
  export default {
    inject: ["color", "font"],
    components: {
      FooterSocial,
    },
  };
</script>
<style scoped>
  .footer {
    background: v-bind("color.toast");
    margin-top: 5rem;
    margin-bottom: -2rem;
  }

  .footer_social {
    padding: 2rem;
  }
</style>
