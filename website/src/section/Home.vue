<template>
  <div class="home">
      <h1>Hello, moi c'est 
       <br /><span>John.</span></h1>
      <h2>Développeur front-end</h2>
      <img src="../assets/me.png">
  </div>
</template>

<script>
export default {
  name: 'Home',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

h2 {
    background: white;
    color: black;
    padding: 10px;
    width: 300px;
    text-align: center;

}


img {
    width: 250px;
    border: 7px solid white;
    border-radius: 50%;
   
}



</style>