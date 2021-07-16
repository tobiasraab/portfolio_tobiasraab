<template>
  <div>
    <div class="quote-container"
      v-bind:style="{backgroundColor: this.backgroundColor, color: this.color}"
      v-html="this.text"
    ></div>
  </div>
</template>

<script>
export default {
  name: 'quote',
  props: ['backgroundColor', 'color', 'text']
  
}
</script>

<style>
  .quote-container{
    display: table-cell;
    vertical-align: middle;

    position: relative;
    width: 100vw;
    height: 40vh;

    text-align: center;

    font-family: 'silkaextra_light';
    font-size: 32px;
  }
</style>