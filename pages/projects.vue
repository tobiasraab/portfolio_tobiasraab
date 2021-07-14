<template>
  <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-16 h-auto max-w-screen-2xl m-auto">
    <projectCard class="projectcard-tag"
      :title="'Wärmepumpe'"
      :label="'UX/UI Design'"
      :image="require('@/assets/images/testImg1.jpg')"
      :description="'Das ist die tolle Beschreibung <br> Ich bin krass, gebt mir euer Geld'"
      :overlayId="'overlayId1'"
    ></projectCard>
     <projectCard class="projectcard-tag"
      :title="'HUBI - Education Kit'"
      :label="'Smart Home'"
      :image="require('@/assets/images/testImg2.jpg')"
      :description="'Das ist die nächste tolle Beschreibung <br> Ich bin krass, gebt mir noch mehr Geld'"
      :overlayId="'overlayId2'"
    ></projectCard>
     <projectCard class="projectcard-tag"
      :title="'Fire Watch'"
      :label="'IoT System'"
      :image="require('@/assets/images/testImg2.jpg')"
      :description="'Das ist die nächste tolle Beschreibung <br> Ich bin krass, gebt mir noch mehr Geld'"
      :overlayId="'overlayId3'"
    ></projectCard>
  </div>
</template>

<script>
import projectCard from './../components/projectCard.vue'

export default {
  name: 'projects',
  layout: 'portfolio',
  components: {
    projectCard
  }
}
</script>

<style>

</style>