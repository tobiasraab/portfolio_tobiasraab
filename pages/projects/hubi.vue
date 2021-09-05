<template>
  <div>
    <quote
      :backgroundColor="'#161616'"
      :color="'#ffffff'"
      :text="'Wie funktioniert Smart Home?'"
    ></quote>
    <textParagraph
      :headline="'Problem'"
      :text="'Problem'"
    ></textParagraph>
    <pictureText
      :headline="'Problem'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: HUBI.'"
      :imageCaption="''"
      :altTag="''"
    ></pictureText>
    <textPicture
      :headline="'UX/UI'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
      :altTag="''"
    ></textPicture>
    <pictureText
      :headline="'Visual Programming Language (VPL)'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
      :altTag="''"
    ></pictureText>
    <textPicture
      :headline="'Unsichtbares Sichtbar'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
      :altTag="''"
    ></textPicture>
    <pictureText
      :headline="'Visual Design'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
      :altTag="''"
    ></pictureText>
    <textPicture
      :headline="'Smart Hub'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
      :altTag="''"
    ></textPicture>
    <pictureText
      :headline="'Prozess'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Diesen Problemen widmet sich das Smart Home Kit: Hubi.'"
      :imageCaption="''"
      :altTag="''"
    ></pictureText>
    <iconPattern
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