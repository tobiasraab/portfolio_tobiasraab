<template>
  <header>
    <!-- top menu -->
    <div id="navTopMenu">
      <!-- links if screen > sm -->
      <div class="hidden sm:inline-flex" id="navTopLinksContainer">
        <NuxtLink class="nav-top-link menuLink" to="/Projects">Projects</NuxtLink>
        <NuxtLink class="nav-top-link menuLink" to="/About">About</NuxtLink>
        <NuxtLink class="nav-top-link menuLink" to="/Contact">Contact</NuxtLink>
      </div>
      <!--menu icon if screen < sm -->
      <div class="nav-toggle-icon-container inline-flex sm:hidden" id="navMenuIconContainer" v-on:click="sideMenu">
        <img class="nav-toggle-icon" src="./../assets/icons/navbarIcon.svg" />
      </div>
    </div>
    <!--side menu -->
    <div class="block sm:hidden" id="navSideMenu">
      <!-- links if screen < sm-->
      <div id="navSideLinksContainer">
        <NuxtLink class="nav-side-link menuLink" to="/Projects">Projects</NuxtLink>
        <NuxtLink class="nav-side-link menuLink" to="/About">About</NuxtLink>
        <NuxtLink class="nav-side-link menuLink" to="/Contact">Contact</NuxtLink>
      </div>
    </div>
  </header>
</template>

<script>
  export default {
    name: 'navigationBar',
    data() {
      return {
        navSideMenuActiv: false
      }
    },
    mounted() {
      const icon = document.getElementById('navMenuIconContainer')
      const sideMenu = document.getElementById('navSideMenu')
      const sideMenuLinkContainer = document.getElementById('navSideLinksContainer')

      window.addEventListener('resize', (e) => {
        if (window.innerWidth >= 420) {
          this.navSideMenuActiv = false

          sideMenu.style.height = '0px'
          sideMenuLinkContainer.style.display = 'none'

          icon.style.transform = "rotate(0deg)";
          icon.style.paddingTop = '12px'
        }
        else if (window.innerWidth < 420) {
          sideMenuLinkContainer.style.display = 'block'

          if(this.navSideMenuActiv === false){
            icon.style.transform = "rotate(0deg)";
            icon.style.paddingTop = '12px'
          }
          else if(this.navSideMenuActiv === true){
            icon.style.transform = "rotate(90deg)"
            icon.style.paddingTop = '16px'
          }
        }
      })
    },
    methods: {
      sideMenu() {
        const icon = document.getElementById('navMenuIconContainer')
        const sideMenu = document.getElementById('navSideMenu')
        const sideMenuLinkContainer = document.getElementById('navSideLinksContainer')

        if (this.navSideMenuActiv === false) {
          this.navSideMenuActiv = true

          sideMenu.style.height = window.innerHeight - 64 - 24 + 'px'

          icon.style.transform = "rotate(90deg)"
          icon.style.paddingTop = '16px'
        } 
        else if (this.navSideMenuActiv === true) {
          this.navSideMenuActiv = false

          sideMenu.style.height = '0px'

          icon.style.transform = "rotate(0deg)";
          icon.style.paddingTop = '12px'
        }
      }
    }
  }

</script>

<style scoped>
  header {
    display: inline-flex;

    position: sticky;
    position: -webkit-sticky;

    height: 64px;
    width: 100vw;
  }
    #navTopMenu {
      z-index: 2;

      width: 100%;
      height: 100%;

      background-color: #0b2027;
    }
      #navTopLinksContainer {
        padding: 0 16px;
      }
        .nav-top-link {
          height: 64px;
          padding: 0 16px;

          font-family: 'silkaregular';
          font-size: 18px;
          line-height: 64px;

          color: white;
        }
        .menuLink:hover{
          color: #ffe600;
        }
        .menuLink:active{
          color: #ffe600;
        }


      .nav-toggle-icon-container {
        z-index: 3;

        height: 100%;
        width: 64px;

        margin-left: 8px;
        padding: 12px;

        transition-duration: 1s;
      }
      .nav-toggle-icon {
        height: 40px;
      }




    #navSideMenu {
      position: absolute;
      left: 0%;
      top: 64px;

      height: 0px;
      width: 80vw;

      transition-duration: 1s;

      background-color: #0b2027;
    }
      #navSideLinksContainer {
        z-index: 1;
        display: block;

        position: absolute;
        bottom: 0px;

        margin-left: 24px;
        margin-bottom: 24px;
      }
        .nav-side-link {
          z-index: 1;
          display: block;

          height: 64px;

          font-family: 'silkaregular';
          font-size: 18px;
          line-height: 64px;

          color: white;
        }
</style>
