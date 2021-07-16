<template>
  <div class="p-12 m-auto max-w-screen-2xl">
    <div class="textPicture-template flex flex-col md:grid gap-8 grid-cols-1 grid-rows-2 md:grid-cols-2 md:grid-rows-1"
      v-bind:style="{backgroundColor: this.backgroundColor}">
      <figure class="row-start-2 md:row-start-1">
        <img class="textPicture-image-template" v-bind:src="this.imageSource" />
        <figcaption>{{this.imageCaption}}</figcaption>
      </figure>
      <div class="textPicture-content-template row-start-1 md:row-start-1">
        <h2>{{this.headline}}</h2>
        <p>{{this.text}}</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'textPicture',
    props: ['imageSource', 'headline', 'text', 'backgroundColor', 'imageCaption'],
    mounted() {}
  }

</script>

<style>
  .textPicture-template {
    width: 100%;
  }

  .textPicture-content-template {
    display: table-cell;
    vertical-align: top;
  }

  .textPicture-image-template {
    display: table-cell;
    width: 100%;
  }

  .textPicture-content-template>h2 {
    font-family: 'silkamedium';
    font-size: 32px;
    color: #061216;

  }

  .textPicture-content-template>p {
    font-family: 'silkaregular';
    font-size: 18px;
  }

  figcaption {
    margin-top: 4px;
    margin-left: 4px;
  }

</style>
