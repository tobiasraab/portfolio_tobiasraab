<template>
  <div>
    <quote class="mt-8"
      :backgroundColor="'#061216'"
      :color="'#ffffff'"
      :text="'Alle. Pfleger. Sind. Arm. Drann. Schock.'"
    ></quote>
    <textPicture class="mt-16"
      :backgroundColor="'#ffffff'"
      :headline="'Header'"
      :text="'Alle. Pfleger. Sind. Arm. Drann. Schock.'"
      :imageSource="require('@/assets/images/pflege/image1.png')"
      :imageCaption="'Anteil der zu Pflegenden nach Altersgruppen'"
    ></textPicture>
    <textPicture class="mt-16"
      :backgroundColor="'#ffffff'"
      :headline="'Header'"
      :text="'Alle. Pfleger. Sind. Arm. Drann. Schock.'"
      :imageSource="require('@/assets/images/pflege/image1.png')"
      :imageCaption="'Anteil der zu Pflegenden nach Altersgruppen'"
    ></textPicture>
  </div>
</template>

<script>
import quote from '../../components/templates/quote.vue'
import textPicture from '../../components/templates/textPicture.vue'

export default {
  name: 'pflege',
  layout: 'project',
  components: {
    quote,
    textPicture
  }
}
</script>

<style>

</style>