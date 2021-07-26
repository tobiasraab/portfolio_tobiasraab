<template>
  <div class="pt-32">
    <h1 class="ml-12 mb-4">Creative Technologist</h1>
    <fullStackDiagram></fullStackDiagram>
  </div>
</template>

<script>
import fullStackDiagram from "~/components/templates/fullStackDiagram.vue";
export default {
  name: "about",
  layout: "project",
  components: {
    fullStackDiagram,
  },
};
</script>

<style scoped>
</style>