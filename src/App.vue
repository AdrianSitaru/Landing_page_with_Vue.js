<template>
  <div id="app">
    <Header/>
    <Herro/>
    <Presentation/>
    <PremiumPart />
  </div>
</template>

<script>

import PremiumPart from "@/components/PremiumPart.vue";
import Header from "./components/Header.vue"
import Herro from "./components/Herro.vue"
import Presentation from "@/components/Presentation.vue";


export default {
  name: 'App',
  components: {
    Herro,
    Header,
    Presentation,
    PremiumPart


  }
}
</script>

<style>
*, app {
  margin: 0;
  padding: 0;
}

</style>
