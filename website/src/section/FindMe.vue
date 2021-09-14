<template>
  <div class="main-container">
    <h1>Contact</h1>
    <div class="find-me-container">
      <img ref="img" src="../assets/images/me.png" alt="Portrait photo John" />
      <div class="icons">
        <FindMeIcons
          class="email"
          title="email"
          content="johndevcode@protonmail.com"
        />
        <FindMeIcons
          title="github"
          content="John-github"
          link="https://github.com/johneyme"
        />
        <FindMeIcons
          title="linkedin"
          content="John E."
          link="https://www.linkedin.com/in/john-eyme/"
        />
        <FindMeIcons
          title="404works"
          content="404Works"
          link="https://www.404works.com/fr/profile/johndevcode"
        />
      </div>
    </div>
  </div>
</template>

<script>
import FindMeIcons from "../components/FindMeIcons";
export default {
  name: "FindMe",
  components: {
    FindMeIcons,
  },
};
</script>

<style scoped>

.main-container {
  padding-bottom: 20em;
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
  background-image: url("../assets/pattern/prism.svg");
  background-size: cover;
  width: 100%;
  height: 650px;
}
h1 {
  font-size: 3em;
  margin-top: 2em;
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
  gap: 2.5em;
}
@media (max-width: 700px) {
  .main-container {
    height:950px
  }
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
