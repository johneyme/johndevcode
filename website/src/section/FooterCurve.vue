<template>
  <div>
    <footer>
      <img src="../assets/logo/johndevcodelogo.png" />
      <div class="vertical-divider"></div>
      <h1>John E.</h1>
    </footer>
  </div>
</template>

<script>
export default {
  name: "FooterCurve",
};
</script>

<style scoped>
footer {
  height: 30vh;
  width: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-flow: row wrap;
  background-color: white;
  user-select: none;
}
.vertical-divider {
  height: 50%;
  width: 2px;
  background-color: #1c1c1c;
}
img {
  width: 300px;
}
h1 {
  color: #1c1c1c;
  font-size: clamp(32px, 5vw, 72px);
  transition: color 0.3s ease-in-out;
}
h1:hover {
  color: #ffb224;
}
@media (max-width: 700px) {
  footer {
    width: 100vw;
  }
  img {
    width: 100px
  }
   
  
}
</style>
