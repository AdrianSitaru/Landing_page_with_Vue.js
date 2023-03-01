<template>
  <div class="footer-part">
    <img src="../assets/spotify_logo2.jpg">
    <nav>
      <a href='item.url' v-for="(item, index) in items1" :key="index">
        {{ item.text }}
      </a>
    </nav>
    <nav>
      <a href='item.url' v-for="(item, index) in items2" :key="index">
        {{ item.text }}
      </a>
    </nav>
    <nav>
      <a href='item.url' v-for="(item, index) in items3" :key="index">
        {{ item.text }}
      </a>
    </nav>
    <div class="social-media">
      <img src="../assets/instagram.png"/>
      <img src="../assets/twitter.png"/>
      <img src="../assets/facebook.png"/>
    </div>
  </div>
</template>
<script>
export default {
  name: "FooterPart",
  data() {
    return {
      items1: [
        {text: 'COMPANIE', url: ''},
        {text: 'Despre', url: ''},
        {text: 'Locuri de Munca', url: ''},
        {text: 'For The Record', url: ''},
      ],
      items2: [
        {text: 'COMUNITATI', url: ''},
        {text: 'Pentru Artisti', url: ''},
        {text: 'Dezvoltatori', url: ''},
        {text: 'Publicitate', url: ''},
        {text: 'Investitori', url: ''},
        {text: 'Furnizori', url: ''},
      ],
      items3: [
        {text: 'LINK-URI URILE', url: ''},
        {text: 'Asistenta', url: ''},
        {text: 'Player Web', url: ''},
        {text: 'Aplicatie Mobila Gratuita', url: ''},
      ]
    }
  }
}
</script>

<style lang="scss">
.footer-part {
  background-color: black;
  color: white;
  height: 500px;
  display: flex;
  flex-wrap: nowrap;
  justify-content: space-evenly;

  img {
    padding: 40px 15px;
    height: 38px;
    width: 110px;
    margin-left: 25px;
  }

  a {
    color: white;
    font-size: 20px;
    text-decoration: none;
    display: block;
    padding: 15px;
  }

  nav {
    display: block;
    padding: 20px;
  }

  .social-media {
    display: flex;
  }

  .social-media img {
    height: 40px;
    width: 40px;
  }
}

</style>