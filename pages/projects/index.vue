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
        :description="'Smart Home Kit, mit welchem der Nutzer Grundlagen des Programmierens erlernt und einen Blick auf den unsichtbaren Datenverkahr im eigenen Zuhause werfen kann.'"
        :overlayId="'overlayId2'"
        :linkedPath="'/projects/hubi'"
      ></projectCard>
      <projectCard
        :title="'Fire Watch'"
        :label="'IoT System'"
        :image="require('@/assets/images/firewatch/sensorImg4.jpg')"
        :description="'System für die Überwachung von Waldbrandrisikogebieten.'"
        :overlayId="'overlayId3'"
        :linkedPath="'/projects/firewatch'"
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