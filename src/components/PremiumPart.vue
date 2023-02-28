<template>
  <div class="premium-section">
    <h2>{{ title }}</h2>
    <p>{{ paragraph }}</p>
    <div class="cards">
      <PremiumCard v-for="card in cards " :key="card.id" :card-data="card"
      />
    </div>
  </div>
</template>

<script>
import PremiumCard from "@/components/PremiumCard.vue";

export default {
  data() {
    return {
      title: 'Alege-ți abonamentul Premium',
      paragraph: 'Asculți nelimitat pe telefon, în boxe și pe alte dispozitive.',
      cards: [
        {
          id: 1,
          span: '3 Luni Gratuite',
          title: 'Individual',
          paragraph: '4.99 EUR/lună după perioada ofertei Un cont',
          images: [
            require('@/assets/tick.png'),
            require('@/assets/tick.png'),
            require('@/assets/tick.png'),
          ],
          description: [
            'Ascultă muzică fără anunțuri',
            'Redai de oriunde chiar și offline',
            'Redare la cerere'
          ],
          button: 'SA INCEPEM',
          terms: 'Doar pentru abonamentul Individual. 4.99 EUR/lună după. Se aplică Termenii și condițiile. Ofertă disponibilă doar pentru utilizatorii care nu au mai încercat versiunea Premium. Oferta se încheie pe 31.12.2022'
        },
        {
          id: 2,
          span: 'O Luna Gratuit',
          title: 'Duo',
          paragraph: '6.49 EUR/lună după perioada ofertei 2 conturi',
          images: [
            require('@/assets/tick.png'),
            require('@/assets/tick.png'),
          ],
          description: [
            '2 conturi Premium pentru un cuplu care locuiește împreună',
            'Asculți muzică fără anunțuri, redai offline și la cerere',
          ],
          button: 'SA INCEPEM',
          terms: 'Se aplică Termenii și condițiile. Luna gratuită nu este disponibilăutilizatorilor care au încercat deja versiunea Premium.'

        },
        {
          id: 3,
          span: 'O Luna Gratuit',
          title: 'Familie',
          paragraph: '7.99 EUR/lună după perioada ofertei Maximum 6 conturi',
          images: [
            require('@/assets/tick.png'),
            require('@/assets/tick.png'),
            require('@/assets/tick.png'),
          ],
          description: [
            '6 conturi Premium pentru membrii familiei care locuiesc împreună',
            'Blochezi muzica cu conținut explicit',
            'Asculți muzică fără anunțuri, redai offline și la cerere'
          ],
          button: 'SA INCEPEM',
          terms: 'Se aplică Termenii și condițiile. Luna gratuită nu este disponibilă utilizatorilor care au încercat deja versiunea Premium.'
        },
        {
          id: 4,
          span: 'O Luna Gratuit',
          title: 'Student',
          paragraph: '2.49 EUR/lună după perioada ofertei Un cont',
          images: [
            require('@/assets/tick.png'),
            require('@/assets/tick.png'),
            require('@/assets/tick.png'),
            require('@/assets/tick.png')
          ],
          description: [
            'Reducere specială pentru studenții eligibili care urmează cursurile unei universități',
            'Ascultă muzică fără anunțuri',
            'Redai de oriunde chiar și offline',
            'Redare la cerere'
          ],
          button: 'SA INCEPEM',
          terms: 'Doar 2.49 EUR/lună după. Ofertă disponibilă doar pentru studenții care urmează cursurile unei instituții acreditate de învățământ superior și care nu au mai încercat Premium. Se aplică Termenii și condițiile.'
        }

      ]

    }
  },
  components: {
    PremiumCard,
  },
  name: "PremiumPartSection"
}
</script>

<style>

.cards {
  display: flex;
  justify-content: space-evenly;
}

.premium-section {
  background-color: #d9d9d9;
  font-size: 20px;
  text-align: center;
}

.premium-section h2 {
  padding: 15px;
  font-size: 40px;
}

</style>