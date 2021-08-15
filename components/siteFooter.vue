<template>
  <footer>
    <div class="footer-container">
      <NuxtLink to="/impressum" class="footer-link">Impressum</NuxtLink>
      <NuxtLink to="/datenschutzerklaerung" class="footer-link">Datenschutzerklärung</NuxtLink>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'siteFooter'
}
</script>

<style>
  footer {
    height: 28px;
    position: relative;
    bottom: 0%;
    z-index: 15;
    width: 100%;
    display: block;
    text-align: center;
    padding-bottom: 6px;
    margin-top: 0px;
  }
  .footer-link{
    margin: 0 8px;
    font-family: 'silkaregular';
    font-size: 13px;
  }
  .footer-container{
    padding: 5px;
    border-top: 1px solid rgb(184, 184, 184);
    border-width: 20%;
    display: inline;
  }
</style>