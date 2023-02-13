<template>
  <div class="Premium__section">
    <h2>Alege-ți abonamentul Premium</h2>
    <h3>Asculți nelimitat pe telefon, în boxe și pe alte dispozitive.</h3>
    <div class="Cards__Container">
      <FirstCard />
      <SecondCard />
      <ThridCard />
      <CardFour />
    </div>
  </div>
</template>
<script>
import CardFour from "./CardFour.vue";
import FirstCard from "./FirstCard.vue";
import SecondCard from "./SecondCard.vue";
import ThridCard from "./ThridCard.vue";
export default {
  name: "PremiumSection",
  components: {
    FirstCard,
    SecondCard,
    ThridCard,
    CardFour,
  },
};
</script>
<style>
.Premium__section {
  background-color: #d9d9d9;
  text-align: center;
  padding: 20px 0px;
}

.Cards__Container {
  display: flex;
  justify-content: space-evenly;
  margin-top: 20px;
}

h2 {
  padding: 30px;
  font-size: 30px;
}
</style>
