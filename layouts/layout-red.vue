<template>
  <div class="layout-template">
    <navigationBar class="nav-bar" />
    <!-- 9A031E FF482A D33F49 E06D06-->
    <Particles
      class="background-template"
      id="tsparticlesRed"
      :options="{
        background: {
          color: {
            value: '#ffffff',
          },
        },
        fpsLimit: 60,
        interactivity: {
          detectsOn: 'canvas',
          events: {
            onClick: {
              enable: false,
              mode: 'push',
            },
            onHover: {
              enable: false,
              mode: 'repulse',
            },
            resize: false,
          },
          modes: {
            bubble: {
              distance: 400,
              duration: 2,
              opacity: 0.8,
              size: 40,
            },
            push: {
              quantity: 4,
            },
            repulse: {
              distance: 200,
              duration: 0.4,
            },
          },
        },
        particles: {
          color: {
            value: '#E06D06',
          },
          links: {
            color: '#E06D06',
            distance: 300,
            enable: true,
            opacity: 0.12,
            width: 1,
          },
          collisions: {
            enable: true,
          },
          move: {
            direction: 'none',
            enable: true,
            outMode: 'bounce',
            random: false,
            speed: 0.1,
            straight: false,
          },
          number: {
            density: {
              enable: true,
              value_area: 800,
            },
            value: 15, // point numbers
          },
          opacity: {
            value: 0.12,
          },
          shape: {
            type: 'circle',
          },
          size: {
            random: true,
            value: 3, // point size
          },
        },
        detectRetina: true,
      }"
    />
    <Nuxt class="layoutNuxt p-0 pt-24"
    />
    <siteFooter class="footer-template"
    ></siteFooter>
  </div>
</template>

<script>
import navigationBar from "../components/navigationBar.vue";
import siteFooter from "../components/siteFooter.vue";


export default {
  components: {
    navigationBar,
    siteFooter
  }
};
</script>
<style scoped>
@import "./../assets/fonts/fontRoman.css";

body {
  font-family: "silkaregular", sans-serif;
  color: #080808;
}
.footer-template {
  position: relative;
  bottom: 0%;
  left: 0%;
  z-index: 2;
}
.layoutNuxt {
  min-height: calc(100vh - 28px - 48px);
  width: 100%;
  z-index: 2;
  margin-bottom: 48px;
  left: 0%;
}
.nav-bar {
  z-index: 4;
}
.background-template{
  display: inline-flex;

  position: fixed;
  top: calc(0% + 64px);

  height: 100vh;
  width: 100vw;

  z-index: 1;
}
</style>
