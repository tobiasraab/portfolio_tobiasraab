<template>
  <div class="diagram-container hidden md:block">
    <!--Background Connector-->
    <div class="diagram-background"></div>

    <div class="diagram-foreground-container flex justify-between">
      <!--Design Stack-->
      <div
        class="
          diagram-design-container
          grid
          gap-6 gap-y-6
          grid-cols-3 grid-rows-2
          justify-items-center
        "
      >
        <div class="diagram-design-item px-3 py-2">
          <h1 class="text-sm lg:text-base xl:text-lg">Research</h1>
        </div>
        <div class="diagram-design-item px-3 py-2">
          <h1 class="text-sm lg:text-base xl:text-lg">UX Design</h1>
        </div>
        <div class="diagram-design-item px-3 py-2">
          <h1 class="text-sm lg:text-base xl:text-lg">UI Design</h1>
        </div>
        <div class="mt- 2xl:mt-2 line row-start-2 col-start-1 col-end-4"></div>
        <h2 class="diagram-label text-sm row-start-2 col-start-2">Full-Stack Design</h2>
      </div>

      <!--Development Stack-->
      <div
        class="
          diagram-development-container
          grid
          gap-6 gap-y-8
          grid-cols-4 grid-rows-2
          justify-items-center
        "
      >
        <div class="diagram-development-item flex flex-wrap content-between px-3 py-2">
          <h1 class="text-sm hidden lg:block lg:text-base xl:text-lg">Frontend Development</h1>
          <h1 class="text-sm hidden md:block lg:hidden">Frontend</h1>
          <ul class="hidden xl:block text-xs 2xl:text-sm ">
            <li>HTML/CSS/JS</li>
            <li>Vue.js</li>
          </ul>
        </div>
        <div class="diagram-development-item flex flex-wrap content-between px-3 py-2">
          <h1 class="text-sm hidden lg:block lg:text-base xl:text-lg">Backend Development</h1>
          <h1 class="text-sm hidden md:block lg:hidden">Backend</h1>
          <ul class="hidden xl:block text-xs 2xl:text-sm">
            <li>Distributed Computing</li>
            <li>IoT-Development</li>
          </ul>
        </div>
        <div class="diagram-development-item flex flex-wrap content-between px-3 py-2">
          <h1 class="text-sm lg:text-base xl:text-lg">Hardware</h1>
          <ul class="hidden xl:block text-xs 2xl:text-sm">
            <li>Physical Computing</li>
            <li>&nbsp;</li>
          </ul>
        </div>
        <div class="diagram-development-item flex flex-wrap content-between px-3 py-2">
          <h1 class="text-sm lg:text-base xl:text-lg">Database</h1>
          <ul class="hidden xl:block text-xs 2xl:text-sm">
            <li>NoSQL</li>
            <li>&nbsp;</li>
          </ul>
        </div>
        <div class="mt- 2xl:mt-2 line-development row-start-2 col-start-1 col-end-5"></div>
        <h2 class="diagram-development-label text-sm row-start-2 col-start-2 col-end-4">
          Full-Stack Development
        </h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'fullStackDiagram',
  layout: 'project'
};
</script>

<style scoped>
ul{
  color: white;
  /* font-size: 16px; */
  font-family: 'silkalight';
}
.diagram-container {
  position: relative;
  top: -6vw;
  left: 0%;
  width: 100vw;
}
.diagram-background {
  z-index: 1;
  position: relative;
  top: 9.75vw;
  width: 100vw;
  height: 8vw;
  background-color: #DCDCDC;
}
.diagram-foreground-container {
  padding: 0 48px;
  position: relative;
  z-index: 5;
  margin-top:0;
  margin-bottom:0;
  margin: auto;
  width: 100%;
}
.diagram-development-label {
  width: 196px;
  background-color: white;
  text-align: center;
}
.diagram-label {
  background-color: white;
  width: 154px;
  text-align: center;
}
.line-development {
  margin-top: 8px;
  height: 1px;
  width: 85%;
  background-color: black;
}
.line {
  margin-top: 8px;
  height: 1px;
  width: 80%;
  background-color: black;
}
.diagram-design-container {
  width: 39%;
}
.diagram-development-container {
  width: 52%;
}
.diagram-design-item {
  background-color: #1a3153;
  width: 11.5vw;
  height: 11.5vw;
  /* padding: 12px 16px; */
  box-shadow: 6px 6px 12px #00000069;
}

.diagram-development-item {
  background-color: #0c1c35;
  width: 11.5vw;
  height: 11.5vw;
  /* padding: 12px 16px; */
  box-shadow: 6px 6px 12px #00000069;
}

h2 {
  font-family: "silkamedium";
  /* font-size: 16px; */
}

h1 {
  color: white;
  font-family: "silkaregular";
  /* font-size: 18px; */
  width: 100%;
}
</style>