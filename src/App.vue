<template>
  <div id="app">
    <Header/>
    <Herro/>
    <div class="features-list">
      <FeatureComponent :data="item" v-for="(item, index) in items" :key="index"/>
    </div>
    <PremiumPart/>
    <FooterPart/>
  </div>
</template>
<script>
import PremiumPart from "@/components/PremiumPart.vue";
import Header from "./components/Header.vue"
import Herro from "./components/Herro.vue"
import FeatureComponent from "@/components/FeatureComponent.vue";
import FooterPart from "@/components/Footer.vue";

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
    FooterPart,
    Herro,
    Header,
    FeatureComponent,
    PremiumPart,
  }
}
</script>
<style lang="scss">
@media only screen and (min-width: 0) {
 .main-header {
   width: 100%;
 }
}

*, #app {
  margin: 0;
  padding: 0;
}

@media only screen and (min-width: 768px) {
  .features-list {
    display: flex;
    justify-content: space-evenly;
  }
}
</style>
