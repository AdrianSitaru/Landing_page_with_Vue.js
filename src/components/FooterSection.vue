<template>
  <div class="Footer">
    <img class="logo" src="../assets/spotify_logo2.jpg" alt="logo" />
    <div>
      <h2>COMPANIE</h2>
      <h3>Despre</h3>
      <h3>Locuri de munca</h3>
      <h3>For the record</h3>
    </div>
    <div>
      <h2>COMUNITATI</h2>
      <h3>Pentru Artisti</h3>
      <h3>Dezvoltatori</h3>
      <h3>Publicitate</h3>
      <h3>Investitori</h3>
      <h3>Furnizori</h3>
    </div>
    <div>
      <h2>LINK-URI UTILE</h2>
      <h3>Asistenta</h3>
      <h3>Player web</h3>
      <h3>Aplicatie mobila gratuita</h3>
    </div>
    <div class="Social__media">
      <img src="../assets/instagram.png" alt="instagram" />
      <img src="../assets/twitter.png" alt="twiter" />
      <img src="../assets/facebook.png" alt="facebok" />
    </div>
  </div>
  <div class="Last__part">
    <a href="#">Legal(informatii juridice)</a>
    <a href="#">Centru de confidentialitate</a>
    <a href="#">Politica de confidentialitate</a>
    <a href="#">Setari pentru cookie-uri</a>
    <a href="#">About Ads(informatii despre reclame)</a>
    <div class="Copiright">
      <div class="Copiright__images">
        <img src="../assets/earth.png" alt="Language" />
        <img src="../assets/copyright.png" alt="Copiright" />
      </div>
      <div class="Copiright__description">
        <p>România(Română)</p>
        <p>2022 Spotify AB</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterSection",
};
</script>
<style scoped>
.Footer {
  background-color: black;
  color: white;
  display: flex;
  padding-bottom: 50px;
  margin-bottom: 0px;
}

.logo {
  padding: 20px;
  width: 100px;
  height: 38px;
}

.Social__media img {
  width: 50px;
  height: 50px;
  padding: 12px;
}

.Last__part {
  background-color: black;
  margin-bottom: 0px;
  height: 100px;
  display: flex;
  justify-content: space-evenly;
}

.Copiright {
  background-color: black;
  display: flex;
}

.Copiright__images img {
  width: 20px;
  height: 20px;
  padding: 5px;
  display: flex;
}

.Copiright__description p {
  color: white;
  font-size: 12px;
  padding: 8px;
}
.Last__part a {
  color: white;
  padding: 15px;
  font-size: 12px;
  text-decoration: none;
}
h2 {
  font-size: 18px;
  text-align: left;
}

h3 {
  font-size: 17px;
  padding: 10px;
  margin-left: 17px;
}
</style>
