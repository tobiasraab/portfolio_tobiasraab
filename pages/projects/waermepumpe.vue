<template>
  <div>
    <quote
      :backgroundColor="'#000000'"
      :color="'#ffffff'"
      :text="'Dashboard für Wärmepumpen'"
    ></quote>
    <pictureItem
      :headline="''"
      :imageSource="require('@/assets/images/waermepumpe/image1.png')"
      :imageCaption="''"
      :altTag="'Dashboard einer Wärmepumpe'"
    ></pictureItem>
    <textPicture
      :headline="'Need'"
      :imageSource="require('@/assets/images/waermepumpe/image6.png')"
      :text="'Wie viel Leistung bringt meine Wärmepumpe? Wie viel Strom hat meine Wärmepumpe letztes Jahr im vergleich zu diesem jahr verbraucht? Gibt es eine Möglichkeit auf alle relevanten Ddaten schnell und einfach zuzugreifen?<br><br>Die Antwort auf diese Fragen bietet das entwickelte Dashboard.'"
      :imageCaption="''"
      :altTag="'User Interface einer Wärmepumpe'"
    ></textPicture>
    <pictureText
      :headline="'Energieumsatz'"
      :imageSource="require('@/assets/images/waermepumpe/image2.png')"
      :text="'In einer Wärmepumpe wird mittels Strom Wärmeenergie gefördert. Je mehr Wärmeenergie aus dem eingespeisten Strom resultiert, desto effizienter ist die Wärmepumpe. Die Ansicht bietet einen intuitiven und klaren Überblick über die verschiedenen Faktoren. In der oberen Hälfte der Darstellung wird der eingespeiste Strom in kWh angegeben. Die Effektivität der Wärmepumpe wird in dem Faktor gemessen, um den sich die eingespeißte Energie erhöht. Dieser wird zwischen den zwei Säulendiagrammen angegeben. In der unteren Hälfte wird die gewonnene Wärmeenergie in rot visualisert.'"
      :imageCaption="''"
      :altTag="'Leistungsverlauf einer Wärmepumpe'"
    ></pictureText>
    <pictureText
      :headline="'Temperatur'"
      :imageSource="require('@/assets/images/waermepumpe/image5.png')"
      :text="'Die Außen- bzw. Bodentemperatur spielt für den Umsatz, den die Wärmepumpe erziehlt, eine wichtige Rolle. Aufgrund dessen kann der Nutzer sich historische Temperaturdaten in seinem Dashboard anzeigen lassen. So kann dieser, aufgrund der Daten aus den vorherigen Jahren, besser abschätzen, wie viel Kosten die Wärmepumpe nächsten Winter vorraussichtlich verursachen wird.'"
      :imageCaption="''"
      :altTag="'Temperaturaufzeichung eines Jahres'"
    ></pictureText>
    <pictureItem
      :headline="'Mid-Fi Variantenbildung'"
      :imageSource="require('@/assets/images/waermepumpe/image8.png')"
      :imageCaption="''"
      :altTag="'Variantenbildung eines Designs'"
    ></pictureItem>
    <pictureItem
      :headline="'High-Fi Variantenbildung'"
      :imageSource="require('@/assets/images/waermepumpe/image7.png')"
      :imageCaption="''"
      :altTag="'High-Fi Variantenbildung'"
    ></pictureItem>
  </div>
</template>

<script>
import quote from "../../components/templates/quote.vue";
import textPicture from "../../components/templates/textPicture.vue";
import pictureText from "../../components/templates/pictureText.vue";
import pictureItem from "../../components/templates/pictureItem.vue";

export default {
  name: "waermepumpe",
  layout: "layout-red",
  components: {
    quote,
    textPicture,
    pictureText,
    pictureItem,
  },
};
</script>

<style>
</style>