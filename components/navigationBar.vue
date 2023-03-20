<template>
  <header>
    <!-- top menu -->
    <div id="navTopMenu">
      <!-- links if screen > sm -->
      <div class="hidden sm:flex justify-between">
        <div class="hidden sm:flex justify-between" id="navTopLinksContainer">
          <NuxtLink class="nav-top-link menuLink" to="/">About</NuxtLink>
          <NuxtLink class="nav-top-link menuLink projects" to="/projects">Projects</NuxtLink>
          <NuxtLink class="nav-top-link menuLink" to="/contact">Contact</NuxtLink>
        </div>
        <h3 class="navTopMenu-currentSite hidden md:block">
          {{ this.showCurrentSite }}
        </h3>
      </div>
      <!--menu icon if screen < sm -->
      <div class="inline-flex sm:hidden" id="navMenuIconContainer" v-on:click="sideMenu">
        <img class="nav-toggle-icon" src="./../assets/icons/navbarIcon.svg" />
      </div>
      <!-- current link if screen < sm -->
      <h3 class="navSideMenu-currentSite inline-flex sm:hidden">{{ this.showCurrentSite }}</h3>
    </div>
    <!--side menu -->
    <div class="block sm:hidden navActiveSideLink" id="navSideMenu">
      <!-- links if screen < sm-->
      <div id="navSideLinksContainer">
        <NuxtLink class="nav-side-link menuLink" id="navSideLinkAbout" to="/">About</NuxtLink>
        <NuxtLink class="nav-side-link menuLink projects" id="navSideLinkProjects" to="/projects">Projects</NuxtLink>
        <NuxtLink class="nav-side-link menuLink" id="navSideLinkContact" to="/contact">Contact</NuxtLink>
      </div>
    </div>
  </header>
</template>

<script>
  export default {
    name: "navigationBar",
    data() {
      return {
        navSideMenuActiv: false,
        currentSite: this.$router.currentRoute.path,
        showCurrentSite: undefined
      };
    },
    mounted() {
      if (this.currentSite == "/projects/waermepumpe") {
        this.showCurrentSite = "Wärmepumpe";
      } else if (this.currentSite == "/projects/hubi") {
        this.showCurrentSite = "HUBI";
      } else if (this.currentSite == "/projects/firewatch") {
        this.showCurrentSite = "Firewatch";
      } else if (this.currentSite == "/projects/raumplaner") {
        this.showCurrentSite = "Raumplaner";
      } else if (this.currentSite == "/projects/unsichtbar") {
        this.showCurrentSite = "(Un)sichtbar";
      } else if (this.currentSite == "/projects/appanalyse") {
        this.showCurrentSite = "Anwendungsanalyse";
      } else if (this.currentSite == "/projects/muenster") {
        this.showCurrentSite = "Ulmer Münster";
      } else if (this.currentSite == "/impressum") {
        this.showCurrentSite = "Impressum";
      } else if (this.currentSite == "/datenschutzerklaerung") {
        this.showCurrentSite = "Datenschutzerklärung";
      } else {
        this.showCurrentSite = "";
      }

      var icon = document.getElementById("navMenuIconContainer");
      var sideMenu = document.getElementById("navSideMenu");
      var sideMenuLinkContainer = document.getElementById("navSideLinksContainer");

      window.addEventListener("resize", (e) => {
        if (window.innerWidth >= 420) {
          this.navSideMenuActiv = false;

          sideMenu.style.height = "0px";
          sideMenuLinkContainer.style.display = "none";

          icon.style.transform = "rotate(0deg)";
          icon.style.paddingTop = "12px";
        } else if (window.innerWidth < 420) {
          sideMenuLinkContainer.style.display = "block";

          if (this.navSideMenuActiv === false) {
            icon.style.transform = "rotate(0deg)";
            icon.style.paddingTop = "12px";
          } else if (this.navSideMenuActiv === true) {
            icon.style.transform = "rotate(90deg)";
            icon.style.paddingTop = "16px";
          }
        }
      });
    },
    methods: {
      sideMenu() {
        const icon = document.getElementById("navMenuIconContainer");
        const sideMenu = document.getElementById("navSideMenu");

        if (this.navSideMenuActiv === false) {
          this.navSideMenuActiv = true;

          sideMenu.style.setProperty("height", "calc(100vh - 88px)")


          icon.style.transform = "rotate(90deg)";
          icon.style.paddingTop = "16px";
        } else if (this.navSideMenuActiv === true) {
          this.navSideMenuActiv = false;

          sideMenu.style.height = "0px";

          icon.style.transform = "rotate(0deg)";
          icon.style.paddingTop = "12px";
        }
      },
    },
    watch: {
      $route: function () {
        this.bigScreenCurrentSite = undefined;
        this.currentSite = this.$router.currentRoute.path;
        console.log(this.currentSite)

        if (this.currentSite == "/projects/waermepumpe") {
          this.showCurrentSite = "Wärmepumpe";
        } else if (this.currentSite == "/projects/hubi") {
          this.showCurrentSite = "HUBI";
        } else if (this.currentSite == "/projects/firewatch") {
          this.showCurrentSite = "Firewatch";
        } else if (this.currentSite == "/projects/raumplaner") {
          this.showCurrentSite = "Raumplaner";
        } else if (this.currentSite == "/projects/unsichtbar") {
          this.showCurrentSite = "(Un)sichtbar";
        } else if (this.currentSite == "/projects/appanalyse") {
          this.showCurrentSite = "Anwendungsanalyse";
        } else if (this.currentSite == "/projects/muenster") {
          this.showCurrentSite = "Ulmer Münster";
        } else if (this.currentSite == "/impressum") {
          this.showCurrentSite = "Impressum";
        } else if (this.currentSite == "/datenschutzerklaerung") {
          this.showCurrentSite = "Datenschutzerklärung";
        } else if (
          this.currentSite == "/projects" ||
          "/about" ||
          "/contact" ||
          "/"
        ) {
          this.showCurrentSite = "";
        }
      },
    },
  };

</script>

<style scoped>
  .navTopMenu-currentSite {
    color: white;
    font-family: "silkamedium", sans-serif;
    font-size: 18px;
    line-height: 64px;
    margin-right: 48px;
  }

  .navSideMenu-currentSite {
    position: absolute;
    color: white;
    font-family: "silkamedium", sans-serif;
    font-size: 18px;
    line-height: 64px;
    right: 24px;
  }

  header {
    display: inline-flex;

    position: fixed;
    top: 0%;

    height: 64px;
    width: 100vw;
  }

  #navTopMenu {
    z-index: 10;

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

    font-family: "silkaregular", sans-serif;
    font-size: 18px;
    line-height: 64px;

    color: white;
  }

  .menuLink:hover {
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

  h1 {
    z-index: 3;

    position: absolute;

    height: 100%;
    width: 64px;

    margin-left: 8px;

    font-family: "silkaregular", sans-serif;
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

    font-family: "silkaregular", sans-serif;
    font-size: 18px;
    line-height: 64px;

    color: white;
  }

  a.nuxt-link-exact-active {
    color: #ffe600;
  }

  a.nuxt-link-active.projects {
    color: #ffe600;
  }

</style>
