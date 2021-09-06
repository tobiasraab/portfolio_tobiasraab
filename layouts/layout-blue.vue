<template>
  <div class="layout-template">
    <navigationBar class="nav-bar" />
    <!-- 1B998B B1DDF1 1B998B 1B998B 0b2027 016FB9-->
    <Particles
      class="background-template"
      id="tsparticlesBlue"
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
            },
            onHover: {
              enable: false,
            },
            resize: false,
          },
        },
        particles: {
          color: {
            value: '#016FB9',
          },
          links: {
            color: '#016FB9',
            distance: 200,
            enable: true,
            opacity: 0.14,
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
            speed: 0.2,
            straight: false,
          },
          number: {
            density: {
              enable: true,
              value_area: 800,
            },
            value: 40, // point numbers
          },
          opacity: {
            value: 0.1,
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
    <Nuxt class="layoutNuxt p-0 pt-24" />
    <siteFooter class="footer-template"></siteFooter>
  </div>
</template>

<script>
import navigationBar from "../components/navigationBar.vue";
import siteFooter from "../components/siteFooter.vue";

export default {
  components: {
    navigationBar,
    siteFooter,
  },
};
</script>
<style scoped>
@import "./../assets/fonts/fontRoman.css";
@import "./../assets/fonts/fontitalic.css";
body {
  font-family: "silkaregular";
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
