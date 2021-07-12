<template>
  <div>
    <navigationBar/>
    <Nuxt />
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
</style>
