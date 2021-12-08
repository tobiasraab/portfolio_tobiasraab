<template>
  <div>
    <div class="quote-container">
      <h1 class="text-3xl md:text-4xl">Tobias Raab</h1>
      <h2 class="text-base md:text-xl md:mt-8">tbs.raab@gmail.com</h2>
    </div>
    <div class="p-12 m-auto max-w-screen-2xl text-template">
      <a href="mailto:tbs.raab@gmail.com">
        <button>Kontaktieren</button>
      </a>
    </div>
  </div>
</template>

<script>



import quote from "~/components/templates/quote.vue";


export default {
  name: "contact",
  layout: "layout-purple",
  components: {
    quote
  },
};
</script>

<style scoped>
.quote-container {
  display: table-cell;
  vertical-align: middle;

  position: relative;
  width: 100vw;
  height: 40vh;

  text-align: center;

  font-family: "silkalight", sans-serif;
  font-size: 32px;

  background-color: #000000;
  color: #ffffff;
}
button {
  position: relative;
  background-color: #0b2027;
  color: white;
  padding-left: 12px;
  font-family: "silkaregular", sans-serif;
  width: 224px;
  height: 44px;
  text-align: left;
  font-size: 14px;
  margin: auto;
  
}
button:hover {
  color: #ffe600;
}
a {
  display: flex;
  margin: auto;

}
h1 {
  font-family: "silkamedium", sans-serif;
  color: #ffffff;
  margin-bottom: 24px;
}
h2 {
  font-family: "silkalight", sans-serif;
  color: #ffffff;
}
</style>