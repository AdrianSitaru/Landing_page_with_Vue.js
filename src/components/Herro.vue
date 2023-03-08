<template>
  <div class="hero-banner">
    <div class="hero-banner-container">
      <h1>0.00 EUR pentru 3 Luni de Premium</h1>
      <h2>
        Bucură-te de muzică fără anunțuri,redare offline și multe altele.
        Anulezi oricând.
      </h2>
      <Buttons/>
      <p>
        Doar pentru abonamentul Individual. 4.99 EUR/lună
        <a href="#">Se aplică Termenii și condițiile.</a> Ofertă disponibilă
        doar pentru utilizatorii care nu au mai încercat versiunea Premium.
        Oferta se încheie pe 31.12.2022.
      </p>
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
@media only screen and (min-width: 0) {
  h1 {
    padding-top: 20px;
    width: 80%;
  }

  .hero-banner-container {
    padding-left: 30px;
  }

  .hero-banner-container p {
    font-size: 12px;
    padding-bottom: 50px;
    padding-left: 30px;
    width: 60vh;
  }

  .hero-banner {
    background-color: rgb(29, 117, 222);
    color: white;

    a {
      text-decoration: none;
      color: white;
    }
    p {
      font-size: 12px;
      margin-bottom: 15px;
    }
  }

  .hero-banner-container h2 {
    padding: 15px 0px;
  }

  .hero-banner h1 {
    padding-top: 50px;
    margin-top: 0px;
    font-size: 38px;
  }
}
</style>