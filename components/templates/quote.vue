<template>
  <div>
    <div
      class="quote-container"
      v-html="this.text"
    ></div>
    <p class="quote-origin">{{ this.origin }}</p>
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

  font-family: "silkalight";
  font-size: 32px;

  background-color: #080808;
  color: #ffffff;
}
.quote-origin {
  margin-top: 4px;
  margin-left: 6px;
}
</style>