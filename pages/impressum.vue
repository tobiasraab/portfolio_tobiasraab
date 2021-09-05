<template>
  <div class="m-auto max-w-screen-2xl px-4 sm:px-8 md:px-16 text-template impressum-container">
    <h1>Impressum</h1>
    <h2>Angaben gemäß § 5 TMG:</h2>
    <p><br>Tobias Raab</p>
    <h3>Postanschrift:</h3>
    <p>Rechbergstraße 42<br>73525 Schwäbisch Gmünd<br></p>
    <h3>Kontakt:</h3>
    <p>Telefon: +49 1575 4622232<br>E-Mail: tbs.raab@gmail.com</p>
    <p></p>
    <p><br></p>
    <p></p>
    <h2>Hinweise zur Website</h2>
    <p></p>
    <h3>Urheberrechtliche Hinweise</h3>
    <p>Tobias Raab<br></p>
  </div>
</template>

<script>
  export default {
    name: "impressum",
    layout: "layout-red",
  };

</script>

<style scoped>
  .impressum-container {
    position: relative;

    text-align: left;

    font-family: "silkaregular";
    font-size: 18px;

    color: #000000;
  }

  h1 {
    font-family: "silkamedium";
    font-size: 32px;
    color: #061216;
  }

  h2 {
    font-family: "silkamedium";
    font-size: 24px;
    color: #061216;
    margin-top: 48px;
  }

  h3 {
    font-family: "silkamedium";
    font-size: 20px;
    color: #061216;
    margin-top: 24px;
  }

  p {
    margin-top: 8px;
    font-family: "silkaregular";
    font-size: 18px;
  }

</style>
