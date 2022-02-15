<template>
  <div>
    <quote
      :backgroundColor="'#161616'"
      :color="'#ffffff'"
      :text="'Der Bau des Ulmer Münsters'"
    ></quote>
    <pictureText
      :headline="'Tangible Interface'"
      :imageSource="require('@/assets/images/muenster/ausstellungseinheit-thumbnail.jpg')"
      :text="'Bei der gezeigten Ausstellungseinheit handelt es sich um eine interaktive Station, welche den Besuchern das Ulmer Münster und seinen Bau veranschaulicht. Hierfür wurde ein Tangible Interface gestaltet. Die Besucher können das Münster eigenständig Bauteil für Bauteil aufbauen. Dabei werden sie mit Informationen zu den jeweiligen Bauetappen versorgt.'"
      :imageCaption="''"
      :altTag="'Ausstellungseinheit Tangible Interface'"
    ></pictureText>
    <videoTemplate
      :src="require('@/assets/videos/muenster.mp4')"
      :headline="'Interaktion'"
    ></videoTemplate>
    <textPicture
      :headline="'Prototyping'"
      :imageSource="require('@/assets/images/muenster/ausstellungseinheit-ablage.jpg')"
      :text="'Mittels Styrodur wurde ein erster Prototyp hergestellt, anhand dessen die Funktionalität und die Interaktion mit der Station getestet werden konnten. Hierbei entstand die Idee, die Teile des Münsters mit Widerstände zu versehen. Wenn ein Bauteil auf ein anderes gestellt wird, verbinden sich die Leitungen der einzelnen Bauteile miteinander. Die darin verbauten Widerstände werden in Reihe geschatlten, wodurch der Arduino messen kann, welche Teile im Model aufgebaut sind. Diese Information wird an das Frontend gesendet, welches dann auf den Baufortschritt reagieren kann. Ein an der Decke hängender Beamer projiziert das Interface auf den Tisch.<br><br>Die Vorteile, die durch einen Prototypen für den Prozess erziehlt werden, wurden in diesem Projekt wiedereinmal sehr deutlich und haben mich in meiner Arbeitsweise bestätigt. Allein durch Konzeption können meiner Meinung nach nicht so gute Ergebnisse erziehlt werden, als durch einem Prototypen, an dem getestet und gearbeitet wird.'"
      :imageCaption="''"
      :altTag="'Ausstellungseinheit Teile Ablage'"
    ></textPicture>
  </div>
</template>

<script>
import quote from "~/components/templates/quote.vue";
import pictureText from "~/components/templates/pictureText.vue";
import textPicture from "~/components/templates/textPicture.vue";
import videoText from "~/components/templates/videoText.vue";
import textVideo from "~/components/templates/textVideo.vue";
import pictureItem from "~/components/templates/pictureItem.vue";
import videoTemplate from "~/components/templates/videoTemplate.vue";

export default {
  name: "muenster",
  layout: "layout-red",
  components: {
    quote,
    pictureText,
    textPicture,
    videoText,
    textVideo,
    pictureItem,
    videoTemplate
  },
};
</script>

<style scoped>
</style>