<template>
  <NuxtLink class="nuxt-link" :to="{ path: this.linkedPath }">
    <div
      v-bind:class="{'loading-hidden': !loaded, 'project-card-container': loaded}"
      class=""
      @mouseenter="mouseEnter()"
      @mouseleave="mouseLeave()"
    >
      <img
      class="project-card-image"
        
        v-bind:src="this.image"
        v-bind:alt="this.altTag"
        v-on:load="imageLoaded"
      />

      <div class="project-card-text-container pr-4 pt-12 sm:pt-10">
        <h2 class="text-xs sm:text-sm">{{ this.label }}</h2>
        <h1 class="text-xl sm:text-2xl">{{ this.title }}</h1>
      </div>
      <div class="project-card-hover-overlay" v-bind:id="this.overlayId">
        <p class="hidden md:block hidden project-card-hover-description">{{ this.description }}</p>
      </div>
    </div>
  </NuxtLink>
</template>

<script>
export default {
  name: "projectCard",
  props: [
    "title",
    "label",
    "image",
    "description",
    "overlayId",
    "linkedPath",
    "altTag",
  ],
  data() {
    return {
      loaded: false,
    };
  },
  components: {
  },
  methods: {
    mouseEnter() {
      document.getElementById(this.overlayId).style.clipPath =
        "polygon(0 0% , 100% 0%, 100% 100%, 0 100%)";
    },
    mouseLeave() {
      document.getElementById(this.overlayId).style.clipPath =
        "polygon(0 78.64% , 100% 70%, 100% 100%, 0 100%)";
    },
    imageLoaded() {
      this.loaded = true;
    },
  },
};
</script>

<style scoped>
.loading-hidden{
  display: none;
}
.nuxt-link {
  height: 400px;
}

.project-card-container {
  display: inline-block;

  height: 400px;
  width: 100%;

  margin: auto;

  cursor: pointer;

  background-color: rgb(214, 214, 214);
  color: white;
}

.project-card-image {
  z-index: 1;

  position: relative;

  height: 85%;
  width: 100%;
}

.project-card-image-loading {
  z-index: 1;

  position: relative;

  height: 85%;
  width: 100%;
  background-color: #0d232b;
}

.project-card-text-container {
  z-index: 3;

  position: relative;
  top: -12%;
  bottom: 0;

  height: 27%;
  width: 100%;

  /* padding-right: 24px; */
  /* padding-top: 32px; */

  text-align: right;

  clip-path: polygon(0 32%, 100% 0, 100% 100%, 0 100%);
  background-color: #1b4e5f;
}

.project-card-hover-overlay {
  z-index: 2;

  position: relative;
  top: -112%;

  height: 100%;
  width: 100%;

  padding: 12px;

  transition-duration: 0.6s;
  clip-path: polygon(0 78.64%, 100% 70%, 100% 100%, 0 100%);

  background-color: rgba(255, 230, 0, 0.95);
}

.project-card-hover-description {
  padding: 2px;

  font-family: "silkamedium";
  font-size: 18px;
  text-align: right;

  color: #0b2027;
}

h1 {
  font-family: "silkaregular";
  /* font-size: 28px; */
}

h2 {
  font-family: "silkalight";
  /* font-size: 14px; */
}
</style>
