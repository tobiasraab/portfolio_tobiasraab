<template>
  <div>
    <quote
      class="mt-8 mb-32"
      :backgroundColor="'#161616'"
      :color="'#ffffff'"
      :text="'Wie funktioniert Smart Home?'"
    ></quote>
    <textParagraph
      class="mb-32"
      :headline="'Problem'"
      :text="'Problem'"
    ></textParagraph>
    <pictureText
      class="mb-32"
      :headline="'Problem'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: HUBI.'"
      :imageCaption="''"
    ></pictureText>
    <textPicture
      class="mb-32"
      :headline="'UX/UI'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
    ></textPicture>
    <pictureText
      class="mb-32"
      :headline="'Visual Programming Language (VPL)'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
    ></pictureText>
    <textPicture
      class="mb-32"
      :headline="'Unsichtbares Sichtbar'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
    ></textPicture>
    <pictureText
      class="mb-32"
      :headline="'Visual Design'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
    ></pictureText>
    <textPicture
      class="mb-32"
      :headline="'Smart Hub'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
    ></textPicture>
    <pictureText
      class="mb-32"
      :headline="'Prozess'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
    ></pictureText>
    <iconPattern class="mb-24"
      :headTitle="'Product Values'"
      :title1="'Transparenz'"
      :icon1="require('@/assets/icons/view.svg')"
      :title2="'Datenschutz'"
      :icon2="require('@/assets/icons/locked.svg')"
      :title3="'Bildung'"
      :icon3="require('@/assets/icons/notebook.svg')"
      :title4="'Kompatibilität'"
      :icon4="require('@/assets/icons/share.svg')"
    ></iconPattern>
  </div>
</template>

<script>
import quote from "~/components/templates/quote.vue";
import pictureText from "~/components/templates/pictureText.vue";
import textPicture from "~/components/templates/textPicture.vue";
import iconPattern from "~/components/templates/iconPattern.vue";
import textParagraph from "~/components/templates/textParagraph.vue";

export default {
  name: "hubi",
  layout: "layout-red",
  components: {
    quote,
    pictureText,
    iconPattern,
    textPicture,
    textParagraph,
  },
};
</script>

<style scoped>
.value-container {
  width: 100%;
  height: 40vh;
  background-color: #161616;
  color: #ffffff;
  padding: 32px;
}
.value-container > h2 {
  width: 100%;
  text-align: center;
  font-family: "silkalight";
  font-size: 32px;
}
</style>