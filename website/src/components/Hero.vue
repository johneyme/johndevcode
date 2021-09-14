<template>
  <main>
    <div class="hero-text">
      <h1 ref="greeting">Hello, moi c'est </h1>
      <h2 ref="name">John.</h2>
      <div ref="profession" @click="goToMe" class="title-wrapper">
        <h3>Développeur Front-end</h3>
      </div>
    </div>
    <aside class="hero-image">
      <img ref="img" src="../assets/images/me.png" alt="Portrait photo John" />
    </aside>
  </main>
</template>

<script>
export default {
  name: "Hero",
  methods: {
    goToMe() {
      document.getElementById("me").scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>

<style scoped>
main {
  display: flex;
  flex-flow: row wrap-reverse;
  justify-content: space-between;
  width: 90%;
}
h1 {
  margin: 0;
  font-weight: 300;
  font-size: clamp(20px, 4vw, 52px);
  margin-left: 15px
}
h2 {
  margin: 0;
  font-size: clamp(100px, 8vw, 140px);
  font-weight: 900;
}
h3 {
  text-align: center;
  font-size: clamp(20px, 2.8vw, 44px);
  margin: 0;
  font-weight: 700;
}
img {
  border: 10px solid white;
  border-radius: 50%;
  width: clamp(200px, 20vw, 20vw);
}
.title-wrapper {
  cursor: pointer;
  margin-top: 1.4em;
  padding: 1em;
  width: 100%;
  background-color: white;
  color: #1c1c1c;
  transition: all 0.2s ease-in-out;
  z-index: 2;
  border-radius: 50px;
}
.title-wrapper:hover {
  background-color: #ffb224;
}

@media (max-width: 700px) {
  main {
    justify-content: center;
    width: 100%;
  }
  img {
    margin-bottom: 2em;
  }
  h2 {
  font-size: clamp(62px, 8vw, 140px);
  font-weight: 900;
}
}
</style>
