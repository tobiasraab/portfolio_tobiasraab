<template>
  <div class="p-12 m-auto max-w-screen-2xl">
    <h2>{{ this.headline }}</h2>
    <div class="video-container">
      <iframe
        class="video"
        width="420"
        height="315"
        v-bind:src="this.src"
        frameborder="0"
        allowfullscreen
      ></iframe>
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
h2 {
  font-family: "silkamedium";
  font-size: 32px;
  color: #061216;
  margin-bottom: 16px;
}
.video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
.video-container {
  position: relative;
  width: 100%;
  height: 0;
  padding-bottom: 56.25%;
}
</style>