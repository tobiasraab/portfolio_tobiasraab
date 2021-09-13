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
      :text="'Die Anzahl der Waldbrände steigt. Und ein Zurückgehen der Brände ist auf Grund des Klimawandels nicht in Sicht. Die Höhe der Risikostufe für einen Waldbrand hängt von verschiedenen Faktoren ab. Zum Beispiel Bodenfeuchtigkeit, Außentemperatur, Luftfeuchtigkeit, Windgeschwindigkeit, usw. Hierfür wurde das IoT-System \'FireWatch\' entwickelt. Es handelt sich hierbei um einen voll funktionsfähigen leicht skallierbaren Produktprototypen. Das System sammelt für den Waldbrandindex relevante Daten und gibt diese dem Nutzer in einem Dashboard aus. Jeder Wald ist mit einem Registrierungscode ausgestattet, sodass der Nutzer seine im Wald gesammelten Daten unkompliziert über einen Code mit Anderen teilen kann.'"
      :imageCaption="''"
      :altTag="'Brennender Wald bei Nacht'"
    ></textPicture>
    <pictureText
      :imageSource="
        require('~/assets/images/firewatch/sensorImg4.jpg')
      "
      :headline="'Sensorstation'"
       :text="'Die Sensorstation wird im Waldboden vergraben, um darin Messungen in verschiedenen Tiefen vorzunehmen. Gemessen werden Bodentemperatur und -feuchtigkeit in der Streuschicht, sowie der Humusschicht. Die gesammelten Daten werden über ein LoRaWAN Modul versendet, um anschließend in einer Datenbank gespeichert zu werden. Die für den Betrieb der Sensorstation benötigte Energie wird für den Prototyp über einen Akku sicher gestellt. Abhängig von der Lage vor Ort kann das System auch um eine Wind- oder Solareinheit weiterentwickelt werden.'"
      :imageCaption="''"
      :altTag="'Sensorstation auf Waldboden'"
    ></pictureText>
    <textPicture
      :imageSource="
        require('~/assets/images/firewatch/firewatch-dashboard-ui.jpg')
      "
      :headline="'Dashboard'"
      :text="'Das Dashboard gibt einen Überblick über die einzelnen Sensoren. Diese können einzeln für sich betrachtet werden. Außerdem wird der Durchschnittswert des ausgewählten Waldes ausgegeben. Ergänzend werden Daten zu Außentemperatur, Wind und Niederschlag dargestellt. Alle wichtigen Daten sind für den Nutzer direkt einsehbar. Durch einen Click auf die jeweilige Region können die Messwerte der einzelnen Sensorstationen eingesehen werden.'"
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
      :headline="'Funktions Prototyp'"
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
