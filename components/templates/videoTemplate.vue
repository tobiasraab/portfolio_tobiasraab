<template>
<!-- TODO: -->
<!-- Use Video tag not youtube!!!!!! -->
  <div class="px-4 sm:px-8 md:px-16 mb-32 md:mb-48 xl:mb-64 m-auto max-w-screen-2xl video-template">
    <h2 v-if="this.headline" class="text-2xl md:text-3xl mb-4 md:mb-8">{{ this.headline }}</h2>
    <div class="video-container">
      <video
        class="video"
        controls
        autoplay
        muted
        loop
      >
        <source v-bind:src="this.src" type="video/mp4">
      </video>
    </div>
  </div>
</template>

<script>
export default {
  name: "videoTemplate",
  props: ["src", "headline"],
};
</script>

<style scoped>
.video-template {
  z-index: 3;
}
h2 {
  z-index: 3;
  position: relative;
  font-family: "silkamedium", sans-serif;
  color: #061216;
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