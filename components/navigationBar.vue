<template>
  <header>
    <!-- top menu -->
    <div id="navTopMenu">
      <!-- links if screen > sm -->
      <div class="hidden sm:inline-flex" id="navTopLinksContainer">
        <NuxtLink class="nav-top-link menuLink" to="/projects"
          v-on:click.native="sideMenu"
        >Projects</NuxtLink>
        <NuxtLink class="nav-top-link menuLink" to="/about"
          v-on:click.native="sideMenu"
        >About</NuxtLink>
        <NuxtLink class="nav-top-link menuLink" to="/contact"
          v-on:click.native="sideMenu"
        >Contact</NuxtLink>
      </div>
      <!--menu icon if screen < sm -->
      <div class="inline-flex sm:hidden" id="navMenuIconContainer" 
        v-on:click="sideMenu"
      >
        <img class="nav-toggle-icon" src="./../assets/icons/navbarIcon.svg" />
      </div>
      <!-- current link if screen < sm -->
      <h1 class="inline-flex sm:hidden">{{this.currentSite}}</h1>
    </div>
    <!--side menu -->
    <div class="block sm:hidden navActiveSideLink" id="navSideMenu">
      <!-- links if screen < sm-->
      <div id="navSideLinksContainer">
        <NuxtLink class="nav-side-link menuLink" id="navSideLinkProjects" to="/projects"
          v-on:click.native="sideMenu"
        >Projects</NuxtLink>
        <NuxtLink class="nav-side-link menuLink" id="navSideLinkAbout" to="/about"
          v-on:click.native="sideMenu"
        >About</NuxtLink>
        <NuxtLink class="nav-side-link menuLink" id="navSideLinkContact" to="/contact"
          v-on:click.native="sideMenu"
        >Contact</NuxtLink>
      </div>
    </div>
  </header>
</template>

<script>
  export default {
    name: 'navigationBar',
    data() {
      return {
        navSideMenuActiv: false,
        currentSite: this.$router.currentRoute.path
      }
    },
    mounted() {
      if(this.currentSite =="/projects/waermepumpe"){
        this.currentSite = "/projects/Wärmepumpe"
      }
      else if(this.currentSite =="/projects/hubi"){
        this.currentSite = "/projects/Hubi"
      }
      else if(this.currentSite =="/projects/firewatch"){
        this.currentSite = "/projects/Firewatch"
      }
      else if(this.currentSite =="/projects/pflege"){
        this.currentSite = "/projects/Pflege"
      }

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
    },
    watch: {
      $route: function() {
        this.currentSite = this.$router.currentRoute.path
        console.log("changed route to",this.currentSite)
      }
    }
  }

</script>

<style scoped>
  header {
    display: inline-flex;

    position: fixed;
    top: 0%;

    height: 64px;
    width: 100vw;
  }
    #navTopMenu {
      z-index: 2;

      /* position: sticky;
      position: -webkit-sticky; */

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




    #navMenuIconContainer {
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


    h1{
      z-index: 3;

      position: absolute;

      height: 100%;
      width: 64px;

      margin-left: 8px;

      font-family: 'silkaregular';
      font-size: 18px;
      line-height: 64px;

      color: white;
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
    a.nuxt-link-active {
      color: #ffe600;
    }
</style>
