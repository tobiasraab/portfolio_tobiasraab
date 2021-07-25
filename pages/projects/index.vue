<template>
  <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-16 h-auto max-w-screen-2xl mt-12 m-auto">
    <projectCard
      :title="'Wärmepumpe'"
      :label="'UX/UI Design'"
      :image="require('@/assets/images/waermepumpe/image4.png')"
      :description="'Wärmepumpen bieten eine nachhaltige Möglichkeit das eigene Haus mit Energie zu versorgen. Die Nutzung einer Wäemepumpe bringt jedoch auch Herausforderungen mit sich. Um diese zu Überwinden wurde das folgende Dashboard entwickelt'"
      :overlayId="'overlayId1'"
      :linkedPath="'/projects/waermepumpe'"
    ></projectCard>
     <projectCard
      :title="'HUBI - Education Kit'"
      :label="'Smart Home'"
      :image="require('@/assets/images/testImg2.jpg')"
      :description="'Das ist die nächste tolle Beschreibung. Ich bin krass, gebt mir noch mehr Geld'"
      :overlayId="'overlayId2'"
      :linkedPath="'/projects/hubi'"
    ></projectCard>
    <projectCard
      :title="'Fire Watch'"
      :label="'IoT System'"
      :image="require('@/assets/images/testImg2.jpg')"
      :description="'Das ist die nächste tolle Beschreibung. Ich bin krass, gebt mir noch mehr Geld'"
      :overlayId="'overlayId3'"
      :linkedPath="'/projects/firewatch'"
    ></projectCard>
    <projectCard
      :title="'Pflege'"
      :label="'Graphic Design'"
      :image="require('@/assets/images/pflege/image1.png')"
      :description="'Das ist die nächste tolle Beschreibung. Ich bin krass, gebt mir noch mehr Geld'"
      :overlayId="'overlayId4'"
      :linkedPath="'/projects/pflege'"
    ></projectCard>
  </div>
</template>

<script>
import projectCard from '../../components/projectCard.vue'

export default {
  name: 'projectList',
  layout: 'portfolio',
  components: {
    projectCard
  }
}
</script>

<style>

</style>