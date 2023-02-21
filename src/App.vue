<template>
  <Header />
  <HeroBanner />
  <Presentation />
  <PremiumSection />
  <FooterSection />
</template>

<script>
import Header from "./components/Header.vue";
import HeroBanner from "./components/HeroBanner.vue";
import Presentation from "./components/Presentation.vue";
import PremiumSection from "./components/PremiumSection.vue";
import FooterSection from "./components/FooterSection.vue";
export default {
  name: "App",
  components: {
    Header,
    HeroBanner,
    Presentation,
    PremiumSection,
    FooterSection,
  },
};
</script>

<style>

</style>
