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
    ></pictureItem>
    <textPicture
      :headline="'Need'"
      :imageSource="require('@/assets/images/waermepumpe/image6.png')"
      :text="'Das entworfene Dashboard hilft dem Nutzer seinen Energiehaushalt im Auge zu behalten. Er bekommt historische Daten zur Effektifität seiner Wärmepumpe angezeigt usw.'"
      :imageCaption="''"
    ></textPicture>
    <pictureText
      :headline="'Energieumsatz'"
      :imageSource="require('@/assets/images/waermepumpe/image2.png')"
      :text="'In einer Wärmepumpe wird mittels Strom Wärmeenergie gefördert. Je mehr Wärmeenergie aus dem eingespeisten Strom resultiert, desto effizienter ist die Wärmepumpe. Die Ansicht bietet einen intuitiven und klaren Überblick über die verschiedenen Faktoren. In der oberen Hälfte der Darstellung wird der eingespeiste Strom in kWh angegeben. Die Effektivität der Wärmepumpe wird in dem Faktor gemessen, um den sich die eingespeißte Energie erhöht. Dieser wird zwischen den zwei Säulendiagrammen angegeben. In der unteren Hälfte wird die gewonnene Wärmeenergie in rot visualisert.'"
      :imageCaption="''"
    ></pictureText>
    <pictureText
      :headline="'Temperatur'"
      :imageSource="require('@/assets/images/waermepumpe/image5.png')"
      :text="'Die Außen- bzw. Bodentemperatur spielt für den Umsatz, den die Wärmepumpe erziehlt, eine wichtige Rolle. Aufgrund dessen kann der Nutzer sich historische Temperaturdaten in seinem Dashboard anzeigen lassen. So kann dieser, aufgrund der Daten aus den vorherigen Jahren, besser abschätzen, wie viel Kosten die Wärmepumpe nächsten Winter vorraussichtlich verursachen wird.'"
      :imageCaption="''"
    ></pictureText>
    <pictureItem
      :headline="'Mid-Fi Variantenbildung'"
      :imageSource="require('@/assets/images/waermepumpe/image8.png')"
      :imageCaption="''"
    ></pictureItem>
    <pictureItem
      :headline="'High-Fi Variantenbildung'"
      :imageSource="require('@/assets/images/waermepumpe/image7.png')"
      :imageCaption="''"
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