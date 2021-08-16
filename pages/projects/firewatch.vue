<template>
  <div>
    <quote
      class="mt-8 mb-32"
      :backgroundColor="'#161616'"
      :color="'#ffffff'"
      :text="'Camp Creek Road Fire:<br>85 Tote'"
      :origin="'Quelle: Government of California (CAL FIRE)'"
    ></quote>
    <textPicture
      class="mb-32"
      :imageSource="
        require('~/assets/images/firewatch/matt-howard-eAKDzK4lo4o-unsplash.jpg')
      "
      :headline="'FireWatch'"
      :text="'Die Anzahl der Waldbrände steigt. ein Zurückgehen der Brände ist durch den Klimawandel nicht in Sicht. Die Höhe der Gefahrenstufe für einen Waldbrand hängt von verschiedenen Faktoren ab. Zum Beispiel Bodenfeuchtigkeit, Außentemperatur, Luftfeuchtigkeit, Windgeschwindigkeit, usw. Hierfür wurde das IoT-System \'FireWatch\' entwickelt. Es handelt sich hierbei um einen voll funktionsfähigen leicht skallierbaren Produktprototypen, inclusive Sensorstationen. Das System sammelt für den Waldbrandindex relevante Daten und gibt dem Nutzer diese in einem Dashboard aus. Jeder Wald ist mit einem Registrierungscode ausgestattet, sodass der Nutzer seine gesammelten Daten über den code unkompliziert mit anderen teilen kann.'"
      :backgroundColor="'#ffffff'"
      :imageCaption="''"
      :altTag="''"
    ></textPicture>
    <pictureText
      class="mb-32"
      :imageSource="
        require('~/assets/images/firewatch/sensorImg4.jpg')
      "
      :headline="'FireWatch'"
      :text="'fsadfadsf'"
      :backgroundColor="'#ffffff'"
      :imageCaption="''"
      :altTag="''"
    ></pictureText>
    <textPicture
      class="mb-32"
      :imageSource="
        require('~/assets/images/firewatch/sensorImg1.jpg')
      "
      :headline="'Sensorstation'"
      :text="''"
      :backgroundColor="'#ffffff'"
      :imageCaption="''"
      :altTag="''"
    ></textPicture>
    <pictureItem
      class="mb-32 hidden md:block"
      :headline="'System'"
      :imageSource="require('@/assets/images/firewatch/system.png')"
      :imageCaption="''"
      :altTag="''"
    ></pictureItem>
    <videoTemplate
      class="mb-32"
      :src="'https://www.youtube-nocookie.com/embed/7PGhk9Zf-bI?&autoplay=1&mute=1&loop=1&playlist=7PGhk9Zf-bI'"
      :headline="'UX/UI (Prototype)'"
    ></videoTemplate>
  </div>
</template>

<script>
import quote from "~/components/templates/quote.vue";
import pictureText from "~/components/templates/pictureText.vue";
import textPicture from "~/components/templates/textPicture.vue";
import productValues from "~/components/templates/productValues.vue";
import textParagraph from "~/components/templates/textParagraph.vue";
import videoTemplate from "~/components/templates/videoTemplate.vue";
import pictureItem from "~/components/templates/pictureItem.vue";

export default {
  name: "firewatch",
  layout: "project",
  components: {
    quote,
    pictureText,
    productValues,
    textPicture,
    textParagraph,
    videoTemplate,
    pictureItem,
  },
};
</script>

<style scoped>
</style>
