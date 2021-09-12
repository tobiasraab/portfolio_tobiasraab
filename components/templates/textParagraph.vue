<template>
  <div class="px-4 sm:px-8 md:px-16 mb-32 md:mb-48 m-auto max-w-screen-2xl text-template">
    <h2 class="text-2xl md:text-3xl" v-if="this.headline">{{ this.headline }}</h2>
    <p class="text-base md:text-lg leading-6 md:leading-7 mt-2 md:mt-4" v-html="this.text"></p>
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
  font-family: "silkamedium", sans-serif;
  color: #061216;
}

.text-template > p {
  font-family: "silkaregular", sans-serif;
}
</style>
