<template>
  <div class="px-4 sm:px-8 md:px-16 mb-32 md:mb-48 m-auto max-w-screen-2xl">
    <div
      class="
        textPicture-template
        flex flex-col-reverse
        lg:grid
        gap-8
        grid-cols-2 grid-rows-1
      "
    >
      <figure class="row-start-1 col-start-2">
        <img class="textPicture-image-template" v-bind:src="this.imageSource" v-bind:alt="this.altTag" />
        <figcaption>{{ this.imageCaption }}</figcaption>
      </figure>
      <div class="textPicture-content-template row-start-1 col-start-1">
        <h2 class="text-xl md:text-3xl">{{ this.headline }}</h2>
        <p class="text-base md:text-lg leading-6 md:leading-7 mt-2 md:mt-4">{{ this.text }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "textPicture",
  props: ["imageSource", "headline", "text", "imageCaption", "altTag"],
  mounted() {},
};
</script>

<style scoped>
.textPicture-template {
  position: relative;
  width: 100%;
  z-index: 3;
}

.textPicture-content-template {
  display: table-cell;
  vertical-align: top;
  background-color: none;
}

.textPicture-image-template {
  display: table-cell;
  width: 100%;
}

.textPicture-content-template > h2 {
  font-family: "silkamedium";
  color: #061216;
}

.textPicture-content-template > p {
  font-family: "silkaregular";
}

figcaption {
  margin-top: 4px;
  margin-left: 4px;
}
</style>
