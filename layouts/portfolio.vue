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