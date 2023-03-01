<template>
  <div id="app">
    <Header/>
    <Herro/>
    <FeatureComponent :data="item" v-for="(item, index) in items" :key="index" />
    <PremiumPart />
  </div>
</template>

<script>

import PremiumPart from "@/components/PremiumPart.vue";
import Header from "./components/Header.vue"
import Herro from "./components/Herro.vue"
import FeatureComponent from "@/components/FeatureComponent.vue";


export default {
  name: 'App',
  data() {
    return {
      items: [
        {
          image: require('@/assets/presentation1.png'),
          description1: 'Descarci muzică.',
          description2: 'Asculți de oriunde.'
        },
        {
          image: require('@/assets/presentation2.png'),
          description1: 'Ascultă muzică fără anunțuri.',
          description2: 'Te bucuri non-stop de muzică.'
        },
        {
          image: require('@/assets/presentation3.png'),
          description1: 'Redă orice melodie.',
          description2: 'Chiar și pe dispozitivul mobil'
        },
        {
          image: require('@/assets/presentation4.png'),
          description1: 'Omiteri nelimitate.',
          description2: 'Doar apeși butonul Înainte.'
        }
      ]
    }
  },
  components: {
    Herro,
    Header,
    FeatureComponent,
    PremiumPart,
  }
}
</script>
<style lang="scss">
*, app {
  margin: 0;
  padding: 0;
}
</style>
