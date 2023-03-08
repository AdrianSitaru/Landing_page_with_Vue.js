<template>
  <header class="main-header">
    <img src="../assets/spotify_logo2.jpg"/>
    <nav>
      <a v-for="item in items" :key="item.id">
        {{ item.name }}<span v-if="item.break">|</span>
      </a>
    </nav>
  </header>
</template>
<script>
export default {
  data() {
    return {
      items: [{
        name: 'Premium',
        route: 'premium',
        id: '23233'
      },
        {
          name: 'Asistență',
          route: 'asistenta',
          id: 'dfffd'
        },
        {
          name: 'Descarcă',
          route: 'Descarcă',
          id: 'sdssda',
          break: true
        },
        {
          name: 'Înregistrează-te',
          route: 'Înregistrează-te',
          id: 'sdsdds',

        },
        {
          name: 'Conectează-te',
          route: 'Conectează-te',
          id: 'deewg'
        }]
    }
  },
  name: "HeaderWeb.vue"
}
</script>

<style lang="scss">
@media only screen and (min-width: 0) {

  .main-header {
    background-color: black;
    width: 100%;
    padding: 10px;
  }

  .main-header img {
    height: 45px;
    width: 125px;
    margin-top: 5px;
    margin-left: 15px;
    cursor: pointer;
  }
}

@media only screen and (min-width: 768px) and (max-width: 991px) {
  .main-header nav {
    display: none;
  }
}

@media only screen and (min-width: 992px) {
  nav {
    display: flex;
    justify-content: space-between;
    color: white;
    margin: 5px 20px;
  }

  .main-header {
    background-color: black;
    height: 60px;
    display: flex;
    justify-content: space-between;
  }

  .main-header img {
    height: 45px;
    width: 125px;
    margin-top: 5px;
    margin-left: 15px;
    cursor: pointer;
  }

  nav span {
    margin-left: 10px;
  }

  nav a {
    padding: 15px;
    margin-bottom: 10px;
  }
}
</style>