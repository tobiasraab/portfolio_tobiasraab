<template>
  <div class="p-12 m-auto max-w-screen-2xl text-template">
    <h2>{{ this.headline }}</h2>
    <p>{{ this.text }}</p>
  </div>
</template>

<script>
export default {
  name: "textParagraph",
  props: ["headline", "text"],
};
</script>

<style scoped>
.text-template {
  width: 100%;
  position: relative;
  z-index: 3;
}

.text-template > h2 {
  font-family: "silkamedium";
  font-size: 32px;
  color: #061216;
}

.text-template > p {
  margin-top: 8px;
  font-family: "silkaregular";
  font-size: 18px;
  line-height: 30px;
}
</style>
