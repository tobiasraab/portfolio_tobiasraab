<template>
  <div class="layout-template">
    <navigationBar class="nav-bar" />
    <!-- 0040A0  -->
    <Particles
      class="background-template"
      id="tsparticlesPurple"
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
            value: '#9067C6',
          },
          links: {
            color: '#9067C6',
            distance: 200,
            enable: true,
            opacity: 0.22,
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
            speed: 0.3,
            straight: false,
          },
          number: {
            density: {
              enable: true,
              value_area: 800,
            },
            value: 80, // point numbers
          },
          opacity: {
            value: 0.22,
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
  z-index: 20;
  margin-bottom: 48px;
  left: 0%;
}
.nav-bar {
  z-index: 3;
}
.background-template{
  display: inline-flex;

  position: fixed;
  top: calc(0% + 64px);

  height: 100vh;
  width: 100vw;
}
</style>
