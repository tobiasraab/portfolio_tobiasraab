<template>
  <div>
    <quote
      :backgroundColor="'#161616'"
      :color="'#ffffff'"
      :text="'Camp Creek Road Fire:<br>85 Tote'"
      :origin="'Quelle: Government of California (CAL FIRE)'"
    ></quote>
    <textPicture
      :imageSource="
        require('~/assets/images/firewatch/matt-howard-eAKDzK4lo4o-unsplash.jpg')
      "
      :headline="'FireWatch'"
      :text="'Die Anzahl der Waldbrände steigt. Und ein Zurückgehen der Brände ist auf Grund des Klimawandels nicht in Sicht. Die Höhe der Gefahrenstufe für einen Waldbrand hängt von verschiedenen Faktoren ab. Zum Beispiel Bodenfeuchtigkeit, Außentemperatur, Luftfeuchtigkeit, Windgeschwindigkeit, usw. Hierfür wurde das IoT-System \'FireWatch\' entwickelt. Es handelt sich hierbei um einen voll funktionsfähigen leicht skallierbaren Produktprototypen. Das System sammelt für den Waldbrandindex relevante Daten und gibt dem Nutzer diese in einem Dashboard aus. Jeder Wald ist mit einem Registrierungscode ausgestattet, sodass der Nutzer seine im Wald gesammelten Daten unkompliziert über einen Code mit Anderen teilen kann.'"
      :imageCaption="''"
      :altTag="'Brennender Wald bei Nacht'"
    ></textPicture>
    <pictureText
      :imageSource="
        require('~/assets/images/firewatch/sensorImg4.jpg')
      "
      :headline="'FireWatch'"
      :text="'fsadfadsf'"
      :imageCaption="''"
      :altTag="'Sensorstation auf Waldboden'"
    ></pictureText>
    <textPicture
      :imageSource="
        require('~/assets/images/firewatch/sensorImg1.jpg')
      "
      :headline="'Sensorstation'"
      :text="''"
      :imageCaption="''"
      :altTag="'Sensorstation'"
    ></textPicture>
    <pictureItem
      class="hidden md:block"
      :headline="'System'"
      :imageSource="require('@/assets/images/firewatch/system.png')"
      :imageCaption="''"
      :altTag="'System Aufbau Visualiserung'"
    ></pictureItem>
    <videoTemplate
      :src="require('@/assets/videos/firewatch_preview.mp4')"
      :headline="'UX/UI (Prototype)'"
    ></videoTemplate>
  </div>
</template>

<script>
import quote from "~/components/templates/quote.vue";
import pictureText from "~/components/templates/pictureText.vue";
import textPicture from "~/components/templates/textPicture.vue";
import textParagraph from "~/components/templates/textParagraph.vue";
import videoTemplate from "~/components/templates/videoTemplate.vue";
import pictureItem from "~/components/templates/pictureItem.vue";

export default {
  name: "firewatch",
  layout: "layout-red",
  components: {
    quote,
    pictureText,
    textPicture,
    textParagraph,
    videoTemplate,
    pictureItem,
  },
};
</script>

<style scoped>
</style>
