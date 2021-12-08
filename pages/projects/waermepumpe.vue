<template>
  <div>
    <quote
      :backgroundColor="'#000000'"
      :color="'#ffffff'"
      :text="'Dashboard für Wärmepumpen'"
    ></quote>
    <pictureItem
      :headline="''"
      :imageSource="require('@/assets/images/waermepumpe/waermepumpe-laptop.jpg')"
      :imageCaption="''"
      :altTag="'Dashboard einer Wärmepumpe'"
    ></pictureItem>
    <textPicture
      :headline="'Problem'"
      :imageSource="require('@/assets/images/waermepumpe/waermepumpe-dashboard.jpg')"
      :text="'Wie viel Leistung bringt meine Wärmepumpe? Wie viel Strom hat meine Wärmepumpe letztes Jahr im Vergleich zu diesem jahr verbraucht? Gibt es eine Möglichkeit auf alle relevanten Daten schnell und einfach zuzugreifen?<br><br>Die Antworten auf diese Fragen bringt das entwickelte Dashboard.'"
      :imageCaption="''"
      :altTag="'User Interface einer Wärmepumpe'"
    ></textPicture>
    <pictureText
       :headline="'Energie-Ansicht'"
      :imageSource="require('@/assets/images/waermepumpe/waermepumpe-dashboard-2.jpg')"
      :text="'In einer Wärmepumpe wird mittels Strom Wärmeenergie gefördert. Je mehr Wärmeenergie aus dem eingespeisten Strom resultiert, desto effizienter ist die Wärmepumpe. Die Energie-Ansicht bietet einen intuitiven und klaren Überblick über die verschiedenen Faktoren. In der oberen Hälfte der Darstellung wird der eingespeiste Strom in kWh angegeben. Die Effektivität der Wärmepumpe wird in dem Faktor gemessen, um den sich die eingespeißte energie nach der Wärmeförderung erhöht. Dieser Faktor (Arbeitszahl) wird zwischen den zwei Säulendiagrammen angegeben. In der unteren Hälfte wird die gewonnene Wärmeenergie in rot visualisert.'"
      :imageCaption="''"
      :altTag="'Leistungsverlauf einer Wärmepumpe'"
    ></pictureText>
    <pictureText
      :headline="'Temperatur-Ansicht'"
      :imageSource="require('@/assets/images/waermepumpe/waermepumpe-temp.jpg')"
      :text="'Die Außen- bzw. Bodentemperatur spielt für den Umsatz den die Wärmepumpe erziehlt eine wichtige Rolle. Aufgrund dessen kann der Nutzer sich auch historische Temperaturdaten in seinem Dashboard anzeigen lassen. So kann dieser, aufgrund der Daten aus den vorherigen Jahren, besser abschätzen, wie viel Kosten die Wärmepumpe nächsten Winter vorraussichtlich verursachen wird.'"
      :imageCaption="''"
      :altTag="'Temperaturaufzeichung eines Jahres'"
    ></pictureText>
    <pictureItem
      :headline="'Mid-Fi Variantenbildung'"
      :imageSource="require('@/assets/images/waermepumpe/waermepumpe-lowfi.jpg')"
      :imageCaption="''"
      :altTag="'Variantenbildung eines Designs'"
    ></pictureItem>
    <pictureItem
      :headline="'High-Fi Variantenbildung'"
      :imageSource="require('@/assets/images/waermepumpe/waermepumpe-highfi.jpg')"
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
