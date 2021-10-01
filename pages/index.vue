<template>
  <div class="pt-0">
    <fullStackDiagram></fullStackDiagram>
    <iconPattern
      class="block md:hidden"
      :headTitle="'Design meets Technology'"
      :title1="'Research'"
      :icon1="require('@/assets/icons/microscope.svg')"
      :altTag1="'Design Research'"
      :title2="'UX Design'"
      :icon2="require('@/assets/icons/touch--interaction.svg')"
      :altTag2="'UX Design'"
      :title3="'UI Design'"
      :icon3="require('@/assets/icons/dashboard.svg')"
      :altTag3="'UI Design'"
      :title4="'Frontend'"
      :icon4="require('@/assets/icons/code2.svg')"
      :altTag4="'Frontend Development'"
      :title5="'Backend'"
      :icon5="require('@/assets/icons/deployment-pattern.svg')"
      :altTag5="'backend Development'"
      :title6="'Database'"
      :icon6="require('@/assets/icons/tree-view--alt.svg')"
      :altTag6="'Database Development'"
      :title7="'Hardware'"
      :icon7="require('@/assets/icons/bot.svg')"
      :altTag7="'Hardware Prototyping'"
    ></iconPattern>
    <pictureText
      :headline="'Tobias Raab'"
      :imageSource="require('@/assets/images/about/tobiasraab-profile.jpg')"
      :text="'Ich bin IoT-Designer und Creative Technologist aus Schwäbisch Gmünd. Aktuell studiere ich an der Hochschule für Gestaltung Schwäbisch Gmünd \'Internet der Dinge - Gestaltung vernetzter Systeme B.A.\'<br>Mein Arbeitsprozess ist geprägt von Design Thinking, sowie dem Ehrgeiz, sinnstiftende Produkte zu entwickeln. Dafür bringe ich weitreichende Kenntnisse im Bereich nutzerzentriertes Design, sowie vernetzte Hard- und Softwareentwicklung ein.'"
      :imageCaption="''"
      :altTag="''"
    ></pictureText>
  </div>
</template>

<script>
import fullStackDiagram from "~/components/fullStackDiagram.vue";
import textParagraph from "~/components/templates/textParagraph.vue";
import pictureText from "~/components/templates/pictureText.vue";
import iconPattern from "~/components/templates/iconPattern.vue"

export default {
  name: "about",
  layout: "layout-blue",
  components: {
    fullStackDiagram,
    textParagraph,
    pictureText,
    iconPattern
  },
};
</script>

<style scoped>
</style>