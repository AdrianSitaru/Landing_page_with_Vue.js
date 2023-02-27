<template>
  <div id="app">
    <Header/>
    <Herro/>
  </div>
</template>

<script>


import Header from "./components/Header.vue"
import Herro from "./components/Herro.vue"


export default {
  name: 'App',
  components: {
    Herro,
    Header,
  }
}
</script>

<style>
*, app {
  margin: 0;
  padding: 0;
}

</style>
