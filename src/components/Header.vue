<template>
  <div class="main-header">
    <img src="../assets/spotify_logo2.jpg">

    <nav>
      <a v-for="item in items" :key="item.id">{{ item.name }} <span v-if="item.break">|</span>
      </a>


    </nav>
  </div>

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

<style>

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

nav {
  display: flex;
  justify-content: space-between;
  color: white;
  padding: 10px;
  margin: 10px;
  width: 500px;
}
nav span {
  margin-left: 10px;
}

</style>