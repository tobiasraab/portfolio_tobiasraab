<template>
  <div>
    <div
      class="
        grid grid-cols-1
        2md:grid-cols-2
        xl:grid-cols-3
        gap-16
        h-auto
        max-w-screen-2xl
        justify-items-center
        mt-12
        m-auto
      "
    >
      <!--TODO: rename images seo friendly and add fill seo friendly altTags-->
      <projectCard
        :title="'Wärmepumpe'"
        :label="'UX/UI Design'"
        :image="require('@/assets/images/waermepumpe/image4.png')"
        :altTag="'lorem ipsum'"
        :description="'Dashboard, mit dessen Hilfe Hausbesitzer alle relevanten Daten über die Leistung ihrer Wärmepumpe einsehen können.'"
        :overlayId="'overlayId1'"
        :linkedPath="'/projects/waermepumpe'"
      ></projectCard>
      <projectCard
        :title="'HUBI - Education Kit'"
        :label="'Smart Home'"
        :image="require('@/assets/images/hubi/hubi-titel.jpg')"
        :description="'Smart Home Kit, mit welchem der Nutzer Grundlagen des Programmierens erlernt und einen Blick auf den unsichtbaren Datenverkehr im eigenen Zuhause werfen kann.'"
        :overlayId="'overlayId2'"
        :linkedPath="'/projects/hubi'"
      ></projectCard>
      <projectCard
        :title="'Fire Watch'"
        :label="'IoT System'"
        :image="require('@/assets/images/firewatch/matt-howard-eAKDzK4lo4o-unsplash2.jpg')"
        :description="'System für die Überwachung von Waldbrandrisikogebieten.'"
        :overlayId="'overlayId3'"
        :linkedPath="'/projects/firewatch'"
      ></projectCard>
      <projectCard
        :title="'Raumplaner'"
        :label="'UX/UI Design'"
        :image="require('@/assets/images/raumplaner/raumplaner-title.jpg')"
        :description="' App, für die Buchung von Zeitslots in verschiedenen Räumen. Damit kann eine organisierte Nutzung von Hochschuleinrichtungen ermöglicht werden.'"
        :overlayId="'overlayId4'"
        :linkedPath="'/projects/raumplaner'"
      ></projectCard>
      <projectCard
        :title="'Anwendungsanalyse'"
        :label="'Research'"
        :image="require('@/assets/images/appanalyse/kernwerk-title.jpg')"
        :description="'Die Fitness-App \'Kernwerk\' wurde hier hinsichtliche der Möglichkeiten analysiert, die der Nutzer hat um sich durch die Anwendung zu navigieren. Die gewonnenen Erkentnisse können genutzt werden um die App für den Nutzer zu optimieren.'"
        :overlayId="'overlayId5'"
        :linkedPath="'/projects/appanalyse'"
      ></projectCard>
      <projectCard
        :title="'Unsichtbares Sichtbar'"
        :label="'Fotografie'"
        :image="require('@/assets/images/unsichtbar/kopfhoererhandy.png')"
        :description="'Dieses Fotoprojekt verfolgt das Thema \'Unsichtbares sichtbar machen\'. Dazu wurden die Vorgänge, die sich in und um elektronische Geräte herum abspielen, sichtbar gemacht.'"
        :overlayId="'overlayId6'"
        :linkedPath="'/projects/unsichtbar'"
      ></projectCard>
    </div>
  </div>
</template>

<script>
import projectCard from "../../components/projectCard.vue";

export default {
  name: "projectList",
  layout: "layout-red-2",
  components: {
    projectCard,
  }
};
</script>

<style scoped>
</style>