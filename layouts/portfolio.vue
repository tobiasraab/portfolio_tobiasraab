<template>
  <div>
    <navigationBar class="nav-bar"/>
    <Nuxt class="layoutNuxt p-8 sm:p-12 md:p-16 lg:p-20" />
  </div>
</template>

<script>
import navigationBar from './../components/navigationBar.vue'

export default {
    components: {
        navigationBar
    }
}
</script>
<style>
@import './../assets/fonts/fontRoman.css';
@import './../assets/fonts/fontitalic.css';
  body {
    font-family: 'silkaregular';
  }
  .layoutNuxt {
    z-index: 1;
  }
  .nav-bar{
    z-index: 10;
  }
</style>
