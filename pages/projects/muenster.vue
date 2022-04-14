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
      :text="'Bei der gezeigten Ausstellungseinheit handelt es sich um eine interaktive Station, welche den Besuchern das Ulmer Münster und seinen Bau veranschaulicht. Hierfür wurde ein spezielles mehrstufiges Tangible Interface entwickelt. Die Besucher können das Münster eigenständig Schritt für Schritt aufbauen. Dabei werden sie mit Informationen zur jeweiligen Bauetappe versorgt.'"
      :imageCaption="''"
      :altTag="'Ausstellungseinheit Tangible Interface'"
    ></pictureText>
    <videoTemplate
      :src="require('@/assets/videos/muenster.mp4')"
      :headline="'Interaktion'"
    ></videoTemplate>
    <textPicture
      :headline="'Prototyping'"
      :imageSource="require('@/assets/images/muenster/work-in-progress.jpg')"
      :text="'Mittels Styrodur wurde ein erster Prototyp hergestellt, anhand dessen die Funktionalität und die Interaktion mit der Station getestet werden konnten. Hierbei entstand die Idee, die Bauteile des Münsters mit Widerständen zu versehen. Wenn ein Bauteil auf ein anderes gestellt wird, verbinden sich die Leitungen der einzelnen Bauteile miteinander. Dadurch werden die verbauten Widerstände parallel hinzugeschatlten. Ein Arduino erkennt nun anhand der veränderten Spannung, welche Teile im Model aufgebaut wurden. Diese Information wird an einen Raspberry Pi geschickt, welcher die Informationen auf dem Interface entsprechend anpasst. Das Interface wird von einem an der Decke hängenden Beamer auf den Tisch projiziert. Die Vorteile, die durch einen schnellen und frühen Prototypen für die weitere Gestaltung generiert werden können, wurden in diesem Projekt sehr deutlich.'"
      :imageCaption="''"
      :altTag="'Work in progress'"
    ></textPicture>
    <pictureItem
      :imageSource="require('@/assets/images/muenster/ausstellungseinheit-ablage.jpg')"
      :altTag="'Ausstellungseinheit Teile Ablage'"
    >
    </pictureItem>
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