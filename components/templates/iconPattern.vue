<template>
  <div class="productValues-template">
    <h1>{{this.headTitle}}</h1>
    <div
      class="
        productValues-container
        grid
        gap-0
        grid-cols-1 grid-rows-4
        md:grid-cols-4 md:grid-rows-1
        place-items-center
        max-w-screen-2xl
      "
    >
      <div class="productValues-item grid-start-1 grid-span-1 mb-28"
        v-if="this.title1"
      >
        <img class="productValues-icon" v-bind:src="this.icon1" />
        <h3 class="productvalues-item-title"><!-- Transparenz -->{{this.title1}}</h3>
      </div>
      <div class="productValues-item grid-start-2 grid-span-1 mb-28"
        v-if="this.title2"
      >
        <img class="productValues-icon" v-bind:src="this.icon2" />
        <h3 class="productvalues-item-title"><!-- Datenschutz -->{{this.title2}}</h3>
      </div>
      <div class="productValues-item grid-start-3 grid-span-1 mb-28"
        v-if="this.title3"
      >
        <img class="productValues-icon" v-bind:src="this.icon3" />
        <h3 class="productvallues-item-title"><!-- Bildung -->{{this.title3}}</h3>
      </div>
      <div class="productValues-item grid-start-4 grid-span-1 mb-28"
        v-if="this.title4"
      >
        <img class="productValues-icon" v-bind:src="this.icon4" />
        <h3 class="productvalues-item-title"><!-- Kompatibilität -->{{this.title4}}</h3>
      </div>
      <div class="productValues-item grid-start-5 grid-span-1 mb-28"
        v-if="this.title5"
      >
        <img class="productValues-icon" v-bind:src="this.icon5" />
        <h3 class="productvalues-item-title"><!-- Kompatibilität -->{{this.title5}}</h3>
      </div>
      <div class="productValues-item grid-start-6 grid-span-1 mb-28"
        v-if="this.title6"
      >
        <img class="productValues-icon" v-bind:src="this.icon6" />
        <h3 class="productvalues-item-title"><!-- Kompatibilität -->{{this.title6}}</h3>
      </div>
      <div class="productValues-item grid-start-7 grid-span-1 mb-28"
        v-if="this.title7"
      >
        <img class="productValues-icon" v-bind:src="this.icon7" />
        <h3 class="productvalues-item-title"><!-- Kompatibilität -->{{this.title7}}</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "productValues",
  props: ['headTitle', 'title1', 'icon1', 'title2', 'icon2', 'title3', 'icon3', 'title4', 'icon4', 'title5', 'icon5', 'title6', 'icon6', 'title7', 'icon7',]
};
</script>

<style scoped>
.productValues-template {
  padding: 48px;
  padding-bottom: 0;
  position: relative;
  z-index: 3;
}
.productValues-container {
  margin: auto;
  padding: 0;
}
h1 {
  position: relative;
  margin-bottom: 96px;
  width: 100%;
  font-size: 32px;
  text-align: center;
  font-family: "silkalight";
}
h3 {
  margin-top: 16px;
  font-size: 24px;
}

img {
  margin: auto;
}

.productValues-template {
  width: 100%;
  color: #ffffff;
  background-color: #161616;
}

.productValues-item {
  display: table;
  justify-content: center;
}

.productValues-icon {
  z-index: 5;
  fill: white;
  height: 50px;
}
</style>
