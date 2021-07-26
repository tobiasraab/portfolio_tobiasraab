<template>
  <div class="p-12 m-auto max-w-screen-2xl">
    <h2>{{ this.headline }}</h2>
    <figure>
      <img v-bind:src="this.imageSource" v-bind:alt="this.altTag"/>
      <figcaption>{{ this.imageCaption }}</figcaption>
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
div > h2 {
  font-family: "silkamedium";
  font-size: 32px;
  color: #061216;
  margin-bottom: 32px;
}
</style>
