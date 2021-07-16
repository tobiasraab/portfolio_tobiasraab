<template>
  <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-16 h-auto max-w-screen-2xl mt-12 m-auto">
    <projectCard
      :title="'Wärmepumpe'"
      :label="'UX/UI Design'"
      :image="require('@/assets/images/waermepumpe/image3.png')"
      :description="'Das ist die tolle Beschreibung. Ich bin krass, gebt mir euer Geld'"
      :overlayId="'overlayId1'"
      :linkedPath="'/waermepumpe'"
    ></projectCard>
     <projectCard
      :title="'HUBI - Education Kit'"
      :label="'Smart Home'"
      :image="require('@/assets/images/testImg2.jpg')"
      :description="'Das ist die nächste tolle Beschreibung. Ich bin krass, gebt mir noch mehr Geld'"
      :overlayId="'overlayId2'"
      :linkedPath="'/hubi'"
    ></projectCard>
    <projectCard
      :title="'Fire Watch'"
      :label="'IoT System'"
      :image="require('@/assets/images/testImg2.jpg')"
      :description="'Das ist die nächste tolle Beschreibung. Ich bin krass, gebt mir noch mehr Geld'"
      :overlayId="'overlayId3'"
      :linkedPath="'/firewatch'"
    ></projectCard>
    <projectCard
      :title="'Pflege'"
      :label="'Graphic Design'"
      :image="require('@/assets/images/pflege/image1.png')"
      :description="'Das ist die nächste tolle Beschreibung. Ich bin krass, gebt mir noch mehr Geld'"
      :overlayId="'overlayId4'"
      :linkedPath="'/pflege'"
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