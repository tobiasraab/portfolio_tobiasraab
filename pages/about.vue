<template>
  <div>
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