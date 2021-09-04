<template>
  <div class="loading-Animation-Container">
    <Particles
      class="background-template"
      id="tsparticlesLoading"
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
              size: 4,
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
              value_area: 4,
            },
            value: 3, // point numbers
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
  </div>
</template>

<script>
export default {
  name: 'loadingAnimation'
}
</script>

<style scoped>
  .loading-Animation-Container{
    z-index: 20;
    position: absolute;
    top: 64px;
    background-color: white;
    height: calc(100vh - 64px);
    width: 100vw;
  }
  #tsparticlesLoading{
    position: relative;
    border-radius: 124px;
    width: 124px;
    height: 124px;
    top: 40%;
    margin: auto;
  }
</style>