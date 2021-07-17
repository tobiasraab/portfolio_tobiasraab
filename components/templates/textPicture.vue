<template>
  <div class="p-12 m-auto max-w-screen-2xl">
    <div class="textPicture-template flex flex-col-reverse md:grid gap-8 grid-cols-2 grid-rows-1"
      v-bind:style="{backgroundColor: this.backgroundColor}">
      <figure class="row-start-1 col-start-2">
        <img class="textPicture-image-template" v-bind:src="this.imageSource" />
        <figcaption>{{this.imageCaption}}</figcaption>
      </figure>
      <div class="textPicture-content-template row-start-1 col-start-1">
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
    font-size: 26px;
    color: #061216;

  }

  .textPicture-content-template>p {
    margin-top: 8px;
    font-family: 'silkaregular';
    font-size: 14px;
  }

  figcaption {
    margin-top: 4px;
    margin-left: 4px;
  }

</style>
