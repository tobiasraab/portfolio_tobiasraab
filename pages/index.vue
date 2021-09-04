<template>
  <div class="pt-0">
    <fullStackDiagram></fullStackDiagram>
    <textPicture
      class="mb-32"
      :headline="'Tobias Raab'"
      :imageSource="require('@/assets/images/about/test.jpg')"
      :text="'Ich bin IoT-Designer und Creative Technologist aus Schwäbisch Gmünd. Aktuell studiere ich an der Hochschule für Gestaltung Schwäbisch Gmünd \'Internet der Dinge - Gestaltung vernetzter Systeme B.A.\''"
      :imageCaption="''"
      :altTag="''"
    ></textPicture>
    <iconPattern
      class="block md:hidden"
      :headTitle="'Design meets Technology'"
      :title1="'Research'"
      :icon1="require('@/assets/icons/microscope.svg')"
      :title2="'UX Design'"
      :icon2="require('@/assets/icons/touch--interaction.svg')"
      :title3="'UI Design'"
      :icon3="require('@/assets/icons/dashboard.svg')"
      :title4="'Frontend'"
      :icon4="require('@/assets/icons/code2.svg')"
      :title5="'Backend'"
      :icon5="require('@/assets/icons/deployment-pattern.svg')"
      :title6="'Database'"
      :icon6="require('@/assets/icons/tree-view--alt.svg')"
      :title7="'Hardware'"
      :icon7="require('@/assets/icons/bot.svg')"
    ></iconPattern>
  </div>
</template>

<script>
import fullStackDiagram from "~/components/fullStackDiagram.vue";
import textParagraph from "~/components/templates/textParagraph.vue";
import textPicture from "~/components/templates/textPicture.vue";
import iconPattern from "~/components/templates/iconPattern.vue"

export default {
  name: "about",
  layout: "layout-blue",
  components: {
    fullStackDiagram,
    textParagraph,
    textPicture,
    iconPattern
  },
};
</script>

<style scoped>
</style>