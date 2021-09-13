<template>
  <div class="main-container">
    <h1>Contact</h1>
    <div class="find-me-container">
      <img
        ref="img"
        src="../assets/images/me.png"
        alt="Portrait photo John"
        @mouseenter="imagePopup"
        @mouseleave="imagePopdown"
      />
      <div class="icons">
      </div>
    </div>
  </div>
</template>

<script>
/*import FindMeIcons from "../components/FindMeIcons";*/
export default {
  name: "FindMe",
  components: {
    /*FindMeIcons,*/
  },

};
</script>

<style scoped>
.main-container {
  padding-bottom: 20em;
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
}
h1 {
  margin-top: 1em;
  text-align: center;
}
img {
  border: 10px solid white;
  border-radius: 50%;
  width: clamp(200px, 20vw, 20vw);
}
.find-me-container {
  margin-top: 3em;
  width: 80vw;
  display: flex;
  flex-flow: row wrap;
  justify-content: space-around;
  align-items: center;
}
.icons {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2em;
}
@media (max-width: 700px) {
  img {
    margin-bottom: 2em;
  }
  .icons {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.2em;
  }
}
</style>