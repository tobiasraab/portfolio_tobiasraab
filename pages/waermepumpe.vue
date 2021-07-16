<template>
  <div>
    <quote
      :backgroundColor="'#000000'"
      :color="'#ffffff'"
      :text="'Das ist sehr inspirierend'"
    ></quote>
  </div>
</template>

<script>
import quote from './../components/templates/quote.vue'
export default {
  name: 'waermepumpe',
  layout: 'project',
  components: {
    quote
  }
}
</script>

<style>

</style>