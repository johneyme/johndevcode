<template>
  <div>
    <ProjectModule class="project-module" />
  </div>
</template>

<script>
import ProjectModule from "../components/ProjectModule.vue";
export default {
  name: "Work",
  components: { ProjectModule },
};
</script>

<style scoped>
div {
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
  background-image: url("../assets/pattern/wavey-fingerprint.svg");
  
}
h1 {
  margin-top: 1em;
  text-align: center;
}
.description {
  width: 60vw;
}
@media (max-width: 700px) {
  div {
    padding: 4em 0em;
  }
  .description {
    text-align: justify;
    width: 90vw;
  }
}
</style>