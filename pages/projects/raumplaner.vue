<template>
  <div>
    <textParagraph
      class="mt-4 md:mt-16"
      :headline="'Raumplaner für Hochschulen'"
      :text="'Während der Coronapandemie können nur eine bestimmte Anzahl an Menschen zur selben Zeit in einen Raum. Um eine problemlose Organisation der Raumbuchung und eine Nachverfolgung der Kontakte zu gewährleisten, wurde diese Smartphone Anwendung designed. Die vorgestellte Raumbuchungsapp ermöglicht es dem Nutzer sich Zeitslots in verschiedenen Räumen zu buchen, um auch in Zeiten der Pandemie nicht auf die Ausstattung - z.B von Fotolaboren - verzichten zu müssen.'"
    ></textParagraph>
    <videoText
      :headline="'Prototype'"
      :src="require('@/assets/videos/raumplaner.mp4')"
      :text="'Im hier vorgestellten Prototyp wird ein klassicher Anwendungsfall vorgestellt. Die Nutzerin benötigt einen Seminarraum um eine Präsentation zu testen. Dafür muss der Raum mit einem Beamer ausgestattet sein. Mithilfe der Filterfunktion der App findet sie schnell geeignete Räume. Im Anschluss fügt sie ihre Projektpartnerin zum Termin hinzu.<br><br>Um in den Raum einzuchecken hält sie ihr Smartphone an den NFC-Reader, welcher an der Tür zum Seminarraum angebracht ist. Dadurch checkt sie in den Raum ein. Verschiedene Sensoren im Raum messen die Luftqualität. Wenn sich diese verschlechtert, wird die Nutzerin mit einer Push-Benachrichtigung auf ihrem Smartphone darauf aufmerksam gemacht.'"
    ></videoText>
    <textPicture
      :headline="'Design System'"
      :imageSource="require('@/assets/images/raumplaner/design-system.jpg')"
      :text="'Variantenbildung und die Beschäftigung mit bestehenden Systemen (Material, Carbon, Polaris), resultierte im erstellten Design System, welches von der App genutzt wird'"
      :imageCaption="''"
      :altTag="'Design System'"
    ></textPicture>
    <pictureText
      :headline="'Mid-Fidelity'"
      :imageSource="require('@/assets/images/raumplaner/raumplaner-varianten.jpg')"
      :text="''"
      :imageCaption="''"
      :altTag="'Mid-Fidelity App Design'"
    ></pictureText>
    <pictureText
      :headline="'High-Fidelity'"
      :imageSource="require('@/assets/images/raumplaner/raumplaner-highfidelity.jpg')"
      :text="''"
      :imageCaption="''"
      :altTag="'High-Fidelity App Design'"
    ></pictureText>
    
  </div>
</template>

<script>
import textPicture from "~/components/templates/textPicture.vue";
import videoText from "~/components/templates/videoText.vue";
import pictureText from "~/components/templates/pictureText.vue";
import textParagraph from "~/components/templates/textParagraph.vue";

export default {
  name: 'raumplaner',
  layout: 'layout-red',
  components: {
    textPicture,
    videoText,
    pictureText,
    textParagraph
  }
}
</script>

<style scoped>

</style>
