<template>
  <div>
    <div class="quote-container"
      v-bind:style="{backgroundColor: this.backgroundColor, color: this.color}"
      v-html="this.text"
    ></div>
    <p class="quote-origin">{{this.origin}}</p>
  </div>
</template>

<script>
export default {
  name: 'quote',
  props: ['backgroundColor', 'color', 'text', 'origin']
  
}
</script>

<style scoped>
  .quote-container{
    display: table-cell;
    vertical-align: middle;

    position: relative;
    width: 100vw;
    height: 40vh;

    text-align: center;

    font-family: 'silkalight';
    font-size: 32px;
  }
  .quote-origin {
    margin-top: 4px;
    margin-left: 6px;
  }
</style>