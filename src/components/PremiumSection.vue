<template>
  <div class="Premium__section">
    <h2>Alege-ți abonamentul Premium</h2>
    <h3>Asculți nelimitat pe telefon, în boxe și pe alte dispozitive.</h3>
    <div class="Cards__Container">
      <PremiumCard v-for="(item, index) in cards"
                   :data="item"
                   :key="index" />
    </div>
  </div>
</template>
<script>
  import PremiumCard from "./PremiumCard.vue";
  export default {
    name: "PremiumSection",
    data () {
      return {
        cards: [
          {
            title: '',
            price: '',
            options: [''],
            description: ``
          },
          {–
            title: '',
            price: '',
            options: [''],
            description: ``
          },
        ]
      }
    },
    components: {
      PremiumCard
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
