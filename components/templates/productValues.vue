<template>
  <div class="productValues-template">
    <h1>Product Values</h1>
    <div class="productValues-container grid gap-8 grid-cols-1 grid-rows-4 md:grid-cols-4 md:grid-rows-1 place-items-center max-w-screen-2xl">
      <div class="productValues-item grid-start-1 grid-span-1 mb-28">
        <img class="productValues-icon" src="~/assets/icons/view.svg" />
        <h3 class="productvalues-item-title">Transparenz</h3>
      </div>
      <div class="productValues-item grid-start-2 grid-span-1 mb-28">
        <img class="productValues-icon" src="~/assets/icons/locked.svg" />
        <h3 class="productvalues-item-title">Datenschutz</h3>
      </div>
      <div class="productValues-item grid-start-3 grid-span-1 mb-28">
        <img class="productValues-icon" src="~/assets/icons/notebook.svg" />
        <h3 class="productvallues-item-title">Bildung</h3>
      </div>
      <div class="productValues-item grid-start-4 grid-span-1 mb-28">
        <img class="productValues-icon" src="~/assets/icons/share.svg" />
        <h3 class="productvalues-item-title">Kompatibilität</h3>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'productValues'
  }

</script>

<style scoped>
  .productValues-template {
    padding: 48px;
    padding-bottom: 0;
  }
  .productValues-container {
    margin: 0;
  }
  h1 {
    position: relative;
    margin-bottom: 96px;
    width: 100%;
    font-size: 32px;
    text-align: center;
    font-family: 'silkalight';
  }
  h3{
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
