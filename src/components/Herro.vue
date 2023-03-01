<template>
  <div class="hero-banner">
    <div class="hero-banner-container">
      <h1>0.00 EUR pentru 3 Luni de Premium</h1>
      <h2>
        Bucură-te de muzică fără anunțuri,redare offline și multe altele.
        Anulezi oricând.
      </h2>
      <p>
        <Buttons/>
        Doar pentru abonamentul Individual. 4.99 EUR/lună
        <a href="#">Se aplică Termenii și condițiile.</a> Ofertă disponibilă
        doar pentru utilizatorii care nu au mai încercat versiunea Premium.
        Oferta se încheie pe 31.12.2022.
      </p>
    </div>
    <div class="image">
      <img src="https://i.scdn.co/image/ab678e040000ed3a34d5c94b798ed61637264101"/>
    </div>
  </div>
</template>
<script>
import Buttons from "@/components/Buttons.vue";
export default {
  name: "HerroPart.vue",
  components: {
    Buttons,
  }
}
</script>
<style lang="scss">
.hero-banner {
  background-color: #df0c8b;
  color: white;
  padding-left: 40px;
  display: flex;
  justify-content: space-between;

  .hero-banner-container {
    max-width: 800px;
    margin-top: 50px;
  }

  .hero-banner-container h2 {
    padding: 15px 0px;
  }

  a {
    text-decoration: none;
    color: white;
}
  .hero-banner h1 {
    padding-top: 50px;
    margin-top: 0px;
    font-size: 38px;
  }

  .hero-banner p {
    font-size: 12px;
    margin-bottom: 15px;
  }

  .image img {
    height: 350px;
    width: 350px;
    padding-right: 30px;
  }
}
</style>