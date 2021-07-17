<template>
  <div>

    <quote class="mt-16 mb-16"
      :backgroundColor="'#000000'"
      :color="'#ffffff'"
      :text="'Dashboard für Wärmepumpen'"
    ></quote>
    <textPicture
      :imageSource="require('@/assets/images/waermepumpe/image3.png')"
      :headline="'Need'"
      :text="'Das entworfene Dashboard hilft dem Nutzer seinen Energiehaushalt im Auge zu behalten. Er bekommt historische Daten zur Effektifität seiner Wärmepumpe angezeigt usw.'"
      :backgroundColor="'#ffffff'"
      :imageCaption="''"
    ></textPicture>
    <pictureText
      :imageSource="require('@/assets/images/waermepumpe/image3.png')"
      :headline="'Need'"
      :text="'Das entworfene Dashboard hilft dem Nutzer seinen Energiehaushalt im Auge zu behalten. Er bekommt historische Daten zur Effektifität seiner Wärmepumpe angezeigt usw.'"
      :backgroundColor="'#ffffff'"
      :imageCaption="''"
    ></pictureText>
  </div>
</template>

<script>
import quote from './../components/templates/quote.vue'
import textPicture from './../components/templates/textPicture.vue'
import pictureText from './../components/templates/pictureText.vue'

export default {
  name: 'waermepumpe',
  layout: 'project',
  components: {
    quote,
    textPicture,
    pictureText
  }
}
</script>

<style>

</style>