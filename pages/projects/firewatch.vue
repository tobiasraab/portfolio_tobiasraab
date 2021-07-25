<template>
  <div>
    <quote
      class="mt-16 mb-32"
      :backgroundColor="'#161616'"
      :color="'#ffffff'"
      :text="'Camp Creek Road Fire:<br>85 Tote'"
      :origin="'Quelle: Government of California (CAL FIRE)'"
    ></quote>
  </div>
</template>

<script>
import quote from "~/components/templates/quote.vue";
import pictureText from "~/components/templates/pictureText.vue";
import textPicture from "~/components/templates/textPicture.vue";
import productValues from "~/components/templates/productValues.vue";
import textParagraph from "~/components/templates/textParagraph.vue";

export default {
  name: "firewatch",
  layout: "project",
  components: {
    quote,
    pictureText,
    productValues,
    textPicture,
    textParagraph,
  },
};
</script>

<style scoped>
</style>