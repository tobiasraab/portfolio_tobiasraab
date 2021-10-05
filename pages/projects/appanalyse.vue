<template>
  <div>
    <textParagraph
      class="mt-4 md:mt-16"
      :headline="'Aufgabe'"
      :text="'Für gewöhnlich wird ein Use-Flow dazu genutzt um herauszuarbeiten, wie sich der Nutzer in der zu entwickelnden Anwendung bewegen können soll. Hier wurde die bereits entwickelte Fitness-App \'KERNWERK\' reverse engineered. Die Visualisierung des Use/Tech-Flows der App ermöglicht es Sackgassen in der Bedienung herauszufinden und neue Verknüpfungen einzubauen, die dem Nutzer die Bedienung erleichtern.'"
    ></textParagraph>
    <pictureItem
      :headline="'Ausgearbeitete Analyse'"
      :imageSource="require('~/assets/images/appanalyse/kernwerk-use-flow.jpg')"
      :imageCaption="''"
      :altTag="'Application Tech-FLow and Use-Flow'"
    ></pictureItem>
  </div>
</template>

<script>
import textParagraph from "~/components/templates/textParagraph.vue";
import pictureItem from "~/components/templates/pictureItem.vue";


export default {
  name: 'appanalyse',
  layout: 'layout-red',
  components: {
    textParagraph,
    pictureItem
  }
}
</script>

<style scoped>

</style>
