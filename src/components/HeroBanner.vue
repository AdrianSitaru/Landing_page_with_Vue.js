<template>
  <div class="HeroBanner">
    <div class="HeroBannerContainer">
      <h1>0.00 EUR pentru 3 Luni de Premium</h1>
      <h2>
        Bucură-te de muzică fără anunțuri,redare offline și multe altele.
        Anulezi oricând.
      </h2>
      <p>
        <Buttons />
        Doar pentru abonamentul Individual. 4.99 EUR/lună
        <a href="#">Se aplică Termenii și condițiile.</a> Ofertă disponibilă
        doar pentru utilizatorii care nu au mai încercat versiunea Premium.
        Oferta se încheie pe 31.12.2022.
      </p>
    </div>
    <div class="image">
      <img class="heroImage" src="../assets/hero_image.jpg" alt="hero_image" />
    </div>
  </div>
</template>
<script>
import Buttons from "./Buttons.vue";
export default {
  name: "TheHeroBanner",
  components: {
    Buttons,
  },
};
</script>

<style scoped>
.HeroBanner {
  background-color: #df0c8b;
  color: white;
  padding-left: 40px;
  display: flex;
}

.HeroBannerContainer {
  max-width: 800px;
  margin-top: 50px;
}

.HeroBannerContainer h2 {
  padding: 15px 0px;
}

.HeroBanner h1 {
  padding-top: 50px;
  margin-top: 0px;
  font-size: 38px;
}

.HeroBanner p {
  font-size: 12px;
}

.heroImage {
  height: 350px;
  width: 350px;
}

.image {
  padding: 50px 150px;
}

a {
  color: white;
  text-decoration: none;
}
</style>
