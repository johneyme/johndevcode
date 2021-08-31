<template>
<div class="banniere">
<img class="logo-johndevcode" src="../assets/johndevcodelogo.png">
 <ul>
    <li>Home</li>
    <li>A propos</li>
</ul>
</div>
</template>

<script>
export default {
  name: 'Banniere',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.banniere {
    display: flex;
    justify-content: space-between;
}


li {
    padding: 10px;
    display: inline-block
}
.logo-johndevcode {
  width: 150px;
  background:white;
}

</style>