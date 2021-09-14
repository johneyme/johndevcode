<template>
  <div class="work-container">
    <h1>Réalisations</h1>
    <div class="project-holder">
      <ProjectModule class="module" />
    </div>
  </div>
</template>

<script>
import ProjectModule from "../components/ProjectModule";
export default {
  name: "Work",
  components: {
    ProjectModule,
  },
};
</script>

<style scoped>
.work-container {
  display: flex;
  flex-flow: column;
  align-items: center;
  background: url("../assets/pattern/wavey-fingerprint.svg");
}
h1 {
  font-size: 3em;
  margin-top: 100px;
}
.module {
  margin-bottom: 10em;
  transition: box-shadow 0.4s ease-in-out;
}
.module:hover {
  box-shadow: 0 0 10px 10px rgba(0, 0, 0, 0.2);
}

.project-holder {
  margin-top: 2em;
}
</style>
