<template>
  <div id="home">
    <Hero class="hero" />
  </div>
</template>

<script>
import Hero from "../components/Hero.vue";

export default {
  name: "Home",
  components: {
    Hero,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#home {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: url("../assets/pattern/home-background-black.png");
  background-size: cover;
}

.hero {
  width: 80vw;
}
</style>
