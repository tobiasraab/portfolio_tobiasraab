<template>
  <div>
    <quote class="mt-16 mb-32"
      :backgroundColor="'#000000'"
      :color="'#ffffff'"
      :text="'Dashboard für Wärmepumpen'"
    ></quote>
    <textPicture class="mb-32"
      :headline="'Need'"
      :imageSource="require('@/assets/images/waermepumpe/image1.png')"
      :text="'Das entworfene Dashboard hilft dem Nutzer seinen Energiehaushalt im Auge zu behalten. Er bekommt historische Daten zur Effektifität seiner Wärmepumpe angezeigt usw.'"
      :backgroundColor="'#ffffff'"
      :imageCaption="''"
    ></textPicture>
    <pictureText class="mb-32"
      :headline="'Energieumsatz'"
      :imageSource="require('@/assets/images/waermepumpe/image6.png')"
      :text="'In einer Wärmepumpe wird mittels Strom Wärmeenergie gefördert. Je mehr Wärmeenergie aus dem eingespeisten Strom resultiert, desto effizienter ist die Wärmepumpe. Die Ansicht bietet einen intuitiven und klaren Überblick über die verschiedenen Faktoren. In der oberen Hälfte der Darstellung wird der eingespeiste Strom in kWh angegeben. Dieser wird benötigt um über die Wärmepumpe Wärmeenergie aus dem Boden zu beziehen. Die Effektivität der Wärmepumpe wird in dem Faktor gemessen, um den sich die eingespeißte Energie erhöht. Dieser wird zwischen den zwei Säulendiagrammen angegeben. In der unteren Hälfte wird die gewonnene Wärmeenergie in rot visualisert.'"
      :backgroundColor="'#ffffff'"
      :imageCaption="''"
    ></pictureText>
    <pictureText class="mb-32"
      :headline="'Temperatur'"
      :imageSource="require('@/assets/images/waermepumpe/image5.png')"
      :text="'Die Außen- bzw. Bodentemperatur spielt für den Umsatz, den die Wärmepumpe erziehlt, eine wichtige Rolle. Aufgrund dessen kann der Nutzer sich historische Temperaturdaten in seinem Dashboard anzeigen lassen. So kann dieser, aufgrund der Daten aus den vorherigen Jahren, besser abschätzen, wie viel Kosten die Wärmepumpe nächsten Winter vorraussichtlich verursachen wird.'"
      :backgroundColor="'#ffffff'"
      :imageCaption="''"
    ></pictureText>
    <pictureTemplate class="mb-32"
      :headline="'Mid-Fi Variantenbildung'"
      :imageSource="require('@/assets/images/waermepumpe/image8.png')"
      :imageCaption="''"
    ></pictureTemplate>
    <pictureTemplate class="mb-32"
      :headline="'High-Fi Variantenbildung'"
      :imageSource="require('@/assets/images/waermepumpe/image7.png')"
      :imageCaption="''"
    ></pictureTemplate>
    <pictureTemplate class="mb-32"
      :headline="'Screens'"
      :imageSource="require('@/assets/images/waermepumpe/image3.png')"
      :imageCaption="''"
    ></pictureTemplate>
  </div>
</template>

<script>
import quote from './../components/templates/quote.vue'
import textPicture from './../components/templates/textPicture.vue'
import pictureText from './../components/templates/pictureText.vue'
import pictureTemplate from './../components/templates/picture.vue'

export default {
  name: 'waermepumpe',
  layout: 'project',
  components: {
    quote,
    textPicture,
    pictureText,
    pictureTemplate
  }
}
</script>

<style>

</style>