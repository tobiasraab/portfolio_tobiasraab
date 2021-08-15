<template>
  <div>
    <navigationBar class="nav-bar"/>
    <Nuxt class="layoutNuxt px-8 pt-8 sm:px-12 pt-12 md:px-16 pt-16 lg:px-20 pt-20" />
    <siteFooter class="footer-template"></siteFooter>
  </div>
</template>

<script>
import navigationBar from './../components/navigationBar.vue'
import siteFooter from './../components/siteFooter.vue'


export default {
  components: {
    navigationBar,
    siteFooter
  }
}
</script>
<style>
@import './../assets/fonts/fontRoman.css';
@import './../assets/fonts/fontitalic.css';
  body {
    font-family: 'silkaregular';
  }
  .footer-template{
    position: relative;
    bottom: 0%;
    left: 0%;
  }
  .layoutNuxt {
    z-index: 1;
  }
  .nav-bar{
    z-index: 10;
  }
</style>
