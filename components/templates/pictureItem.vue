<template>
  <div class="px-4 sm:px-8 md:px-16 mb-32 md:mb-48 m-auto max-w-screen-2xl pictureItem-template">
    <h2 class="text-xl md:text-3xl mb-4 md:mb-8" v-if="this.headline">{{ this.headline }}</h2>
    <figure>
      <img v-bind:src="this.imageSource" v-bind:alt="this.altTag"/>
      <figcaption v-if="this.imageCaption">{{ this.imageCaption }}</figcaption>
    </figure>
  </div>
</template>

<script>
export default {
  name: "pictureitem",
  props: ["headline", "imageSource", "imageCaption", "altTag"],
};
</script>

<style scoped>
figcaption{
  position: relative;
  z-index: 3;
}
.pictureItem-template{
  position: relative;
  z-index: 3;
}
div > h2 {
  font-family: "silkamedium", sans-serif;
  color: #061216;
}
img {
  margin: auto;
}
</style>
