<template>
  <header class="nav-container justify-between">
    <div class="nav-links-container">
      <div class="nav-link-container">
        <NuxtLink class="nav-link" to="/Projects">Projects</NuxtLink>
      </div>
      <div class="nav-link-container">
        <NuxtLink class="nav-link" to="/About">About</NuxtLink>
      </div>
      <div class="nav-link-container">
        <NuxtLink class="nav-link" to="/Contact">Contact</NuxtLink>
      </div>
    </div>
    <div class="nav-toggle-icon-container">
      <img class="nav-toggle-icon" src="./../assets/icons/navbarIcon.svg"/>
    </div>
  </header>
</template>

<script>
  export default {

  }

</script>

<style scoped>
  header {
    background-color: #0b2027;
    height: 64px;
    width: 100vw;
    position: sticky;
    position: -webkit-sticky;
    display: inline-flex;
  }
  .nav-links-container{
    padding: 0 16px;
    display: inline-flex;
  }
  .nav-link-container {
    padding: 0 16px;
  }
  .nav-link {
    font-family: 'silkaregular';
    font-size: 18px;
    line-height: 62px;
    color: white;
  }
  .nav-link:hover {
    color: #ffe600;
  }
  .nav-toggle-icon-container{
    height: 100%;
    width: 64px;
    padding: 12px;
  }
  .nav-toggle-icon{
    height: 40px;
  }
</style>
