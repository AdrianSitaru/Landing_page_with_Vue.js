<template>
  <div class="footer-part">
    <img src="../assets/spotify_logo2.jpg"/>
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
    <figure class="social-media">
      <img src="../assets/instagram.png"/>
      <img src="../assets/twitter.png"/>
      <img src="../assets/facebook.png"/>
    </figure>
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
  @media only screen and (min-width: 0) {

    background-color: black;
    a {
      color: white;
      font-size: 16px;
      font-weight: 400;
      text-decoration: none;
      display: block;
      padding: 15px;
    }
    img {
      padding: 40px 15px;
      height: 38px;
      width: 110px;
      margin-left: 25px;
    }

    @media only screen and (min-width: 768px) {
    .social-media img {
        height: 38px;
        width: 38px;
      }
    }
  }
}

footer-part {
  background-color: black;
  color: white;
  height: 500px;
  display: flex;
  flex-wrap: nowrap;
  justify-content: space-evenly;


  nav {
    display: block;
    padding: 20px;
  }

  .social-media {
    display: flex;
  }


}

</style>