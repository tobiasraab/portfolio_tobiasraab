<template>
    <div class="diagram-container hidden md:block md:mt-32">
      <!--Background Connector-->
      <h1>Design meets Technology</h1>
      <div class="diagram-background"></div>
      <div class="diagram-foreground-container flex justify-between">
        <!--Design Stack-->
        <div class="
          diagram-design-container
          grid
          gap-6 gap-y-6
          grid-cols-3 grid-rows-2
          justify-items-center
        ">
          <div class="diagram-design-item px-3 py-2">
            <h2 class="text-sm lg:text-base xl:text-lg">Research</h2>
            <img class="diagram-icon hidden lg:block" src="~/assets/icons/microscope.svg" alt="Design Research"/>
          </div>
          <div class="diagram-design-item px-3 py-2">
            <h2 class="text-sm lg:text-base xl:text-lg">UX Design</h2>
            <img class="diagram-icon hidden lg:block" src="~/assets/icons/touch--interaction.svg" alt="UX Design"/>
          </div>
          <div class="diagram-design-item px-3 py-2">
            <h2 class="text-sm lg:text-base xl:text-lg">UI Design</h2>
            <img class="diagram-icon hidden lg:block" src="~/assets/icons/dashboard.svg" alt="UI Design"/>
          </div>
          <div class="mt-2 2xl:mt-2.5 line row-start-2 col-start-1 col-end-4"></div>
          <h3 class="diagram-label text-sm row-start-2 col-start-2">
            Full-Stack Design
          </h3>
        </div>

        <!--Development Stack-->
        <div class="
          diagram-development-container
          grid
          gap-6 gap-y-8
          grid-cols-4 grid-rows-2
          justify-items-center
        ">
          <div class="
            diagram-development-item
            flex flex-wrap
            content-between
            px-3
            py-2
          ">
            <h2 class="text-sm lg:text-base xl:text-lg">Frontend</h2>
            <ul class="hidden xl:block text-xs 2xl:text-base">
              <li>HTML/CSS/JS</li>
              <li>Vue.js</li>
            </ul>
          </div>
          <div class="
            diagram-development-item
            flex flex-wrap
            content-between
            px-3
            py-2
          ">
            <h2 class="text-sm lg:text-base xl:text-lg">Backend</h2>
            <ul class="hidden xl:block text-xs 2xl:text-base">
              <li>Distributed Computing</li>
              <li>IoT-Development</li>
            </ul>
          </div>
          <div class="
            diagram-development-item
            flex flex-wrap
            content-between
            px-3
            py-2
          ">
            <h2 class="text-sm lg:text-base xl:text-lg">Database</h2>
            <ul class="hidden xl:block text-xs 2xl:text-base">
              <li>NoSQL</li>
              <li>SQL</li>
            </ul>
          </div>
          <div class="
            diagram-development-item
            flex flex-wrap
            content-between
            px-3
            py-2
          ">
            <h2 class="text-sm lg:text-base xl:text-lg">Hardware</h2>
            <ul class="hidden xl:block text-xs 2xl:text-base">
              <li>Physical Computing</li>
              <li>C++</li>
            </ul>
          </div>
          <div class="
            mt-2
            2xl:mt-2.5
            line-development
            row-start-2
            col-start-1 col-end-5
          "></div>
          <h3 class="
            diagram-development-label
            text-sm
            row-start-2
            col-start-2 col-end-4
          ">
            Full-Stack Development
          </h3>
        </div>
      </div>
    </div>
</template>

<script>
  export default {
    name: "fullStackDiagram",
  };

</script>

<style scoped>
  .diagram-container {
    position: relative;
    width: 100%;
  }

  .diagram-background {
    z-index: 2;
    position: absolute;
    top: 8%;
    width: 100%;
    height: 8vw;
    background-color: #dcdcdc;
  }

  .diagram-foreground-container {
    padding: 0 48px;
    position: relative;
    z-index: 2;
    margin-top: 0;
    margin-bottom: 0;
    margin: auto;
    width: 100%;
  }

  .diagram-icon {
    width: calc((100% - 24px) / 100 * 36);
    margin: auto;
    margin-top: calc((100% - 24px) / 100 * 30);
  }

  ul {
    color: white;
    /* font-size: 16px; */
    font-family: "silkalight", sans-serif;
  }


  .diagram-development-label {
    width: 204px;
    background-color: white;
    height: 24px;
    text-align: center;
  }

  .diagram-label {
    background-color: white;
    height: 24px;
    width: 154px;
    text-align: center;
  }

  .line-development {
    height: 1px;
    min-width: 85%;
    width: calc(100% - 96px);
    background-color: black;
  }

  .line {
    height: 1px;
    min-width: 85%;
    width: calc(100% - 96px);
    background-color: black;
  }

  .diagram-design-container {
    width: 39%;
  }

  .diagram-development-container {
    width: 52%;
  }

  .diagram-design-item {
    background-color: #0c1c35
      /* #1a3153 */
    ;
    width: 11.5vw;
    height: 11.5vw;
    /* padding: 12px 16px; */
    box-shadow: 6px 6px 12px #00000069;
  }

  .diagram-development-item {
    background-color: #1a3153
      /* #0c1c35 */
    ;
    width: 11.5vw;
    height: 11.5vw;
    /* padding: 12px 16px; */
    box-shadow: 6px 6px 12px #00000069;
  }

  h1 {
    position: absolute;
    top: -80px;
    font-family: "silkamedium", sans-serif;
    font-size: 32px;
    color: #061216;
    z-index: 2;
    margin-left: 44px;
  }

  h3 {
    font-family: "silkamedium", sans-serif;
    color: black;
    /* font-size: 16px; */
  }

  h2 {
    color: white;
    font-family: "silkaregular", sans-serif;
    /* font-size: 18px; */
    width: 100%;
  }

</style>
