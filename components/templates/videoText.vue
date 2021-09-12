<template>
  <div class="px-4 sm:px-8 md:px-16 mb-32 md:mb-48 m-auto max-w-screen-2xl">
    <div class="
        textPicture-template
        flex flex-col-reverse
        lg:grid
        gap-8
        grid-cols-2 grid-rows-1
      ">
      <div class="video-container">
        <video class="video" controls autoplay muted>
          <source v-bind:src="this.src" type="video/mp4">
        </video>
      </div>
      <div class="textPicture-content-template row-start-1 col-start-2">
        <h2 class="text-xl md:text-3xl">{{ this.headline }}</h2>
        <p class="text-base md:text-lg leading-6 md:leading-7 mt-2 md:mt-4" v-html="this.text"></p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "textPicture",
    props: ["src", "headline", "text"],
  };

</script>

<style scoped>
  .textPicture-template {
    width: 100%;
    position: relative;
    z-index: 3;
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
    font-family: "silkamedium", sans-serif;
    color: #061216;
  }

  .textPicture-content-template>p {
    font-family: "silkaregular", sans-serif;
  }

  figcaption {
    margin-top: 4px;
    margin-left: 4px;
  }

  .video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

  .video-container {
    z-index: 3;

    position: relative;
    width: 100%;
    height: 0;
    padding-bottom: 56.25%;
  }

</style>
