<template>
<div id="app">
  <!--<Menu />-->
  <Home id="home" class="section" />
  <Me id="me" class="section" />
  <Work id="work" class="section" />
  <FindMe id="find-me" class="section" />
  <FooterCurve id="footer-curve" class="section" />
 
 </div>
</template>

<script>

import Home from './section/Home.vue'
import Me from "./section/Me";
import Work from "./section/Work";
import FindMe from "./section/FindMe";
import FooterCurve from "./section/FooterCurve";
/*
import Menu from './components/Menu.vue'*/

export default {
  name: 'App',
  components: {
    Home,
    Me,
    Work,
    FindMe,
    FooterCurve, 
    /*Menu, 
     
     
    
    */
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap');

* {
  font-family: Roboto, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
 
}

body {
  margin: 0;
  padding: 0;
  background-color: #1c1c1c;
  color: white;
  position: relative;
  overflow-x: hidden;
  scroll-behavior: smooth;
}

</style>
