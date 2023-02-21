<template>
  <div class="main-header">
    <img class="main-logo" src="../assets/spotify_logo2.jpg" alt="image" />
    <span class="hamb-menu">|||</span>

    <nav>
      <a v-for="item in items"
         :href="item.route">
        {{ item.name }}
        <span v-if="item.break">|</span>
      </a>
    </nav>

  </div>
</template>

<script>
  export default {
    name: "TheHeader",
    data () {
      return {
        items: [
          {
            name: 'Premium',
            route: 'premium'
          },
          {
            name: 'Asistență',
            route: 'asistenta'
          },
          {
            name: 'Descarcă',
            route: '',
            break: true
          },
          {
            name: 'Înregistrează-te',
            route: ''
          },
          {
            name: 'Conectează-te',
            route: ''
          },
        ]
      }
    }
  };
</script>

<style lang="scss">
  .main-header {
    @media only screen and (min-width: 0) {
      background-color: black;
      display: flex;
      justify-content: space-between;
      .main-logo {
        height: 45px;
        width: 125px;
        margin-top: 5px;
        margin-left: 15px;
        cursor: pointer;
      }
      .hamb-menu {
        color: white;
        transform: rotate(90deg);
      }
      nav {
        margin-top: 10px;
        display: flex;
        justify-content: space-between;
        list-style: none;
        color: white;
      }
    }

    @media only screen and (min-width: 992px) {
      .hamb-menu {
        display: none;
      }
    }
  }
</style>
