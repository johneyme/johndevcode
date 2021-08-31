<template>
  <Banniere />
  <Home />
 
</template>

<script>
import Banniere from './section/Banniere.vue'
import Home from './section/Home.vue'

export default {
  name: 'App',
  components: {
    Home,
    Banniere
  }
}
</script>

<style>

body {
  background: black;
  color: white
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin-top: 30px;
 
}
</style>
