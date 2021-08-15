<template>
  <div class="pt-0">
    <textPicture
      class="mb-32"
      :headline="'Tobias Raab'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Ich bin Designer und Creative Technologist aus Schwäbisch Gmünd. Aktuell studiere ich an der Hochschule für Gestaltung Schwäbisch Gmünd \'Internet der Dinge - Gestaltung vernetzter Systeme B.A.\''"
      :backgroundColor="'#ffffff'"
      :imageCaption="''"
    ></textPicture>
    <fullStackDiagram></fullStackDiagram>
    <background></background>
  </div>
</template>

<script>
import fullStackDiagram from "~/components/fullStackDiagram.vue";
import textParagraph from "~/components/templates/textParagraph.vue";
import textPicture from "~/components/templates/textPicture.vue";
import background from "~/components/templates/background.vue"

export default {
  name: "about",
  layout: "project",
  components: {
    fullStackDiagram,
    textParagraph,
    textPicture,
    background
  },
};
</script>

<style scoped>
#siteFooterAbout {
  display: block;
  position: relative;
  left: 0%;
  margin-top: 96px;
}
</style>