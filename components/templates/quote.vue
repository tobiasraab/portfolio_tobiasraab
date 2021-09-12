<template>
  <div class="mb-32 md:mb-48">
    <h2
      class="quote-container leading-10 p-16 text-2xl md:text-3xl"
      v-html="this.text"
    ></h2>
    <p class="quote-origin" v-if="this.origin">{{ this.origin }}</p>
  </div>
</template>

<script>
export default {
  name: "quote",
  props: ["text", "origin"],
};
</script>

<style scoped>
.quote-container {
  z-index: 3;
  position: relative;
  display: table-cell;
  vertical-align: middle;

  position: relative;
  width: 100vw;
  height: 40vh;

  text-align: center;

  font-family: "silkalight", sans-serif;

  background-color: #080808;
  color: #ffffff;
}
.quote-origin {
  position: relative;
  z-index: 3;
  margin-top: 4px;
  margin-left: 6px;
}
</style>