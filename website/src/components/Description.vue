<template>
  <article>
    <h2>A propos de moi</h2>
    <p>
      Je suis développeur Front-end junior, je crée des applications et des sites web responsives. 
      Maitrisant le triptyque de base, à savoir <span>HTML, CSS, JavaScript</span>, je me suis pris 
      d'affection pour le framework <span>VueJs</span>. Je conçois aussi des sites vitrines ou e-commerce via
      la CMS <span>Wordpress</span>, afin de livrer un site esthétique et fonctionnel dans un court laps de temps.
    </p>

    <p>
      Les systèmes d'exploitation que j'utilise sont Linux et Windows.
      </p>
      <p>
      De mon temps libre, j'expérimente de nouvelles technologies de développement et j'apprends à utiliser certains
      logiciels de traitement d'images et de montage vidéo.
    </p>
    <ul>

      <li>
        <img id="html5" class="img-logo" src="../assets/icons/html.png" alt="html5" />
      </li>
      <li>
        <img id="css3" class="img-logo" src="../assets/icons/css.png" alt="css3" />
      </li>
      <li>
        <img id="javascript" class="img-logo" src="../assets/icons/javascript.png" alt="javascipt" />
      </li>
      <li>
        <img id="vuejs" class="img-logo" src="../assets/icons/vuejs.png" alt="vuejs" />
      </li>
      <li>
        <img id="wordpress" class="img-logo" src="../assets/icons/wordpress.png" alt="wordpress" />
      </li>
  
    </ul>
  </article>
</template>

<script>
export default {
  name: "Description",
  
}
</script>

<style scoped>
article {
  background: rgba(0,0,0,0.7);
  padding: 30px;
  border-radius: 30px
}
p {
  font-size: clamp(18px, 1.2vw, 1.2vw);
  line-height: 2;
  color: white;
  font-weight: bold
}
h2 {
  font-size: clamp(24px, 3vw, 3vw);
  font-weight: 300;
  margin: 0;
}
ul {
  margin-top: clamp(3em, 4vw, 4vw);
  list-style-type: none;
  display: flex;
  justify-content: space-around;
}
img {
  height: 45px;
}

#vuejs {
  margin-top: 5px;
  height: 40px;
}
span {
  background: rgba(255,255,255,0.80);
  color: black;
  border-radius: 3px;
  padding: 4px
}

@media (max-width: 700px) {
  p {
    padding: 25px;
  }
  article {
    background: rgba(0,0,0,0.6);
  }
  #vuejs {
    margin-top: 10px;
  height: 35px;
  margin-left: 15px;
}
#wordpress {
    margin-top: 8px;
  height: 38px;
  margin-left: 15px;
}
}
</style>