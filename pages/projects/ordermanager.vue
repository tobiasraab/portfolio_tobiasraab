<template>
  <div>
    <quote
      :backgroundColor="'#000000'"
      :color="'#ffffff'"
      :text="'<span style=\'line-height: 1.5\'>Wie können wir Logistikleitern dabei helfen,<br>Störungen und Anomalien in Aufträgen frühzeitig zu erkennen und zu lösen?</span>'"
    ></quote>
    <pictureText
      :headline="'Research'"
      :imageSource="require('@/assets/images/ordermanager/Order-Manager-Interview.jpg')"
      :text="'Nachdem die Gestaltungs-Challenge im Team definiert wurde, begann die Research Phase des Design Thinking Prozesses. Darin entwarf ich zunächst ein Interview, um unsere Nutzer und deren Bedürfnisse kennen zu lernen. Hierbei stellte sich heraus, dass hinter dem Wunsch nach Übersichtlichkeit und Datenvisualisierung ein anderes Nutzerbedürfniss steht: Auftretende Probleme und Anomalien schnell und zuverlässig zu erkennen.'"
      :imageCaption="''"
      :altTag="'Interview Fragebogen'"
    ></pictureText>
    <textPicture
      :headline="'Creation'"
      :imageSource="require('@/assets/images/ordermanager/NAiSE-Order-Manager-Error.jpg')"
      :text="'Bei der Erstellung der UI-Komponenten konnte ich auf den zuvor von mir erstellten NAiSE Design Guide zurückgreifen. Das Interface ist in einen Overview und einen Detailview unterteilt. Im Detailview können einzelne Order genau betrachtet und Probleme schnell ausgemacht werden. Die Unterteilung eines Holistic Orders in mehrere Transport Order wird hierin auch visuell aufgegriffen.'"
      :imageCaption="''"
      :altTag="'Visual System'"
    ></textPicture>
    <pictureText
      :headline="'Testing'"
      :imageSource="require('@/assets/images/ordermanager/vue-code.jpg')"
      :text="'Um den Order Manager auch im Produktivbetrieb testen zu können, wird dieser nun in die Anwendung der Firma NAiSE GmbH integriert. Das daraus resultierende Feedback hilft uns dabei, diesen weiter auf die Bedürfnisse unserer Nutzer anzupassen.'"
      :altTag="'Screen with Vue.js Code'"
    ></pictureText>
    <pictureItem
      :headline="'Holistic Order Manager'"
      :imageSource="require('~/assets/images/ordermanager/NAiSE-Order-Manager.jpg')"
      :imageCaption="''"
      :altTag="'Application Tech-FLow and Use-Flow'"
    ></pictureItem>
  </div>
</template>

<script>
import quote from "~/components/templates/quote.vue";
import pictureText from "~/components/templates/pictureText.vue";
import textPicture from "~/components/templates/textPicture.vue";
import pictureItem from "~/components/templates/pictureItem.vue";


export default {
  name: 'ordermanager',
  layout: 'layout-red',
  components: {
    quote,
    pictureText,
    textPicture,
    pictureItem
  }
}
</script>

<style scoped>

</style>
