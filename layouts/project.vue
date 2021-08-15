<template>
  <div class="layout-template">
    <navigationBar class="nav-bar"/>
    <Nuxt class="layoutNuxt p-0 pt-24" />
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
    min-height: calc(100vh - 28px - 48px);
    width: 100%;
    z-index: 1;
    margin-bottom: 48px;
    left: 0%;
  }
  .nav-bar{
    z-index: 10;
  }
</style>
