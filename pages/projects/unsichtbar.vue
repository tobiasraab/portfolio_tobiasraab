<template>
  <div>
    <quote
      :backgroundColor="'#000000'"
      :color="'#ffffff'"
      :text="'Unsichtbares sichtbar machen'"
    ></quote>
    <pictureItem
      :headline="''"
      :imageSource="require('~/assets/images/unsichtbar/esp.png')"
      :imageCaption="'WiFi'"
      :altTag="'Wifi-connection ESP-32'"
    ></pictureItem>
    <pictureItem
      :headline="''"
      :imageSource="require('~/assets/images/unsichtbar/espstrom.png')"
      :imageCaption="'Strom'"
      :altTag="'ESP-32 Power'"
    ></pictureItem>
    <pictureItem
      :headline="''"
      :imageSource="require('~/assets/images/unsichtbar/kopfhoerer2.png')"
      :imageCaption="'Ton'"
      :altTag="'Kopfhörer Audio'"
    ></pictureItem>
    <pictureItem
      :headline="''"
      :imageSource="require('~/assets/images/unsichtbar/kopfhoererhandy.png')"
      :imageCaption="'Bluetooth'"
      :altTag="'Bluetooth connection'"
    ></pictureItem>
    <pictureItem
      :headline="''"
      :imageSource="require('~/assets/images/unsichtbar/ladekabel.png')"
      :imageCaption="'Strom'"
      :altTag="'strom in Ladekabel'"
    ></pictureItem>
  </div>
</template>

<script>
import pictureItem from "~/components/templates/pictureItem.vue";
import quote from "~/components/templates/quote.vue";



export default {
  name: 'unsichtbar',
  layout: 'layout-red',
  components: {
    pictureItem,
    quote
  }
}
</script>

<style scoped>

</style>
