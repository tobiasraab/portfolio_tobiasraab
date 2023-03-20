<template>
  <div>
    <quote
      :backgroundColor="'#161616'"
      :color="'#ffffff'"
      :text="'Wie funktioniert ein Smart Home System?'"
    ></quote>
    <pictureText
      :headline="'Problem'"
      :imageSource="require('@/assets/images/hubi/question.png')"
      :text="'Wie funktioniert Smart Home? Was passiert mit meinen Daten? Kann ich das als Leie überhaupt? Wie kann ich mein Zuhause präzise und einfach automatisieren um mein Leben so zu vereinfachen, wie ich es möchte? <br><br>Das sind Fragen, die sich Menschen stellen, bevor sie sich ein Smart Home System aufbauen. Das Smart Home Kit HUBI bietet darauf die passende Lösung.'"
      :imageCaption="''"
      :altTag="'Fragezeichen'"
    ></pictureText>
    <textVideo
      :headline="'Unsichtbares Sichtbar'"
      :text="'Für den Laien ist die Vorstellung von Datenverkehr in einem Netzwerk etwas sehr abstraktes. Um dem Nutzer ein Verständniss für die vielen unsichtbaren Datenpakete zu vermitteln, die er in seinem Smart Home Netzwerk versendet, wurde die Netzwerkansicht entwickelt. Diese visualisiert alle im Smart Home registrierten Geräte und ermöglicht dem Nutzer die im Netzwerk verschickten Daten einzusehen. Wenn zum Beispiel die ZigBee-Fernbedienung gedrückt wird, zeigt die Netzwerkansicht parallel dazu, wie ein Datenpaket von der Fernbedienung zum Smart Hub gesendet wird. Zusätzlich leuchten die LEDs im Case des Smart Hubs auf.'"
      :src="require('@/assets/videos/hubi_network.mp4')"
    ></textVideo>
    <videoText
      :headline="'UX/UI'"
      :src="require('@/assets/videos/hubi_uxui.mp4')"
      :text="'Damit dem Nutzer eine möglichst intuitive und verständliche Möglichkeit geboten wird sein Smart Home zu programmieren, wurde eine neue grafische Programmiersprache entwickelt. Diese basiert, ähnlich wie Node-RED, auf dem Prinzip von verschiedenen Knoten. Jedes steuerbare Gerät im Netzwerk wird als Knoten visualisert. Wenn es sich um einen Aktor handelt, kann der Nutzer Daten an das Gerät senden. Wenn es sich bei dem Gerät um einen Sensor, zum Beispiel zur Überwachung der Temperatur, handelt, kann der Nutzer die empfangenen Daten in seinem Programmier-Flow verarbeiten. Mit verschiedenen Funktionen (if-Nodes, send-Nodes, loops) kann der Nutzer sein Smarthome individuell an seine Bedürfnisse anpassen.'"
    ></videoText>
     <pictureItem
      :headline="'Visual Programming Language (VPL)'"
      :imageSource="require('@/assets/images/hubi/hubi-vpl-ui.jpg')"
      :altTag="'Visual Programming Language Interface'"
    >
    </pictureItem>
    <textPicture
      :headline="'Hardware'"
      :imageSource="require('@/assets/images/hubi/hubi-hardware.png')"
       :text="'Im entworfenen Case ist ist ein Raspberry Pi verbaut, welcher einen Web Server hostet, mit dem der Nutzer sein Smart Home steuert. Dadurch dass der Server direkt vom Smart Hub gehostet wird verlassen die Daten des Nutzers das eigene Heimnetzwerk nicht. Dadurch kann der Datenschutz sicher gestellt werden. Um die Kommunikation mit verschiedenen Smart Home Devices zu ermöglichen ist eine ZigBee-Antenne mit in das System integriert. Des Weiteren erhält der Nutzer über die verbauten LEDs ein visuelles Feedback, wenn Daten vom Smart Hub versendet oder empfangen werden.'"
      :imageCaption="''"
      :altTag="'Smart Home Basis Station'"
    ></textPicture>
    <pictureText
      :headline="'Software'"
      :imageSource="require('@/assets/images/hubi/hubi-backend-code.jpg')"
      :text="'Das Backend besteht aus einem Node Server welcher auf dem Rapberry Pi gehostet wird. Da die graphische Programmieroberfläche mit dem Schwerpunkt Smart Home gestaltet wurde, gab es noch keine existierende Software, welche den gestelten Anforderungen an Gerätekompatibilität und Nutzerfreundlichkeit mit Schwerpunkt Smart Home gerecht wurde. Aufgrund dessen musste ein von Grund auf neues Programm entwickelt werden. Dieses bildet das Gehirn des Systems. Von ihm werden die vom Nutzer erstellten Flows zur Heimautomation verwaltet und umgesetzt. Hierfür genutze Technologien sind unter anderem: Express.js, socket.io, mqtt. Umgesetzt wurde die neue Programmiersprache mit JavaScript. Das Frontend ist mit dem Framework vue.js gestaltet und kommuniziert über eine Rest Schnittstelle, ergänzend zu socket.io, mit dem Backend.'"
      :imageCaption="''"
      :altTag="'Node.js Backend Code'"
    ></pictureText>
     <textPicture
      :headline="'Visual Design'"
      :imageSource="require('@/assets/images/hubi/hubi-visual.png')"
      :text="'Das Maskottchen unterstützt den Nutzer inerhalb der Anwendung mit hilfreichen Tipps und Erklärungen, sowie einem Tutorial zum Kennen lernen der verschiedenen Funktionen. Die Verpackung enthält verschiedene Motive, welche den Aspekt Netzwerktechnik visualiserien. Datenpakete werden hierbei verbildlicht zwischen Sechsecken hin und her geschickt.'"
      :imageCaption="''"
      :altTag="'Visual System'"
    ></textPicture>
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
import videoText from "~/components/templates/videoText.vue";
import textVideo from "~/components/templates/textVideo.vue";
import pictureItem from "~/components/templates/pictureItem.vue";

export default {
  name: "hubi",
  layout: "layout-red",
  components: {
    quote,
    pictureText,
    iconPattern,
    textPicture,
    videoText,
    textVideo,
    pictureItem
  },
};
</script>

<style scoped>
</style>