<template>
  <div class="Card__container">
    <span>3 Luni Gratuite</span>
    <h3>Individual</h3>
    <p>4.99 EUR/lună după perioada ofertei Un cont</p>
    <div class="Container__line"></div>
    <div class="Content__container">
      <div class="Image__Container">
        <img src="../assets/tick.png" alt="image" />
        <img src="../assets/tick.png" alt="image" />
        <img src="../assets/tick.png" alt="image" />
      </div>
      <div class="Description">
        <p>Ascultă muzică fără anunțuri</p>
        <p>Redai de oriunde chiar și offline</p>
        <p>Redare la cerere</p>
      </div>
    </div>
    <button class="btn">SĂ ÎNCEPEM</button>
    <p id="terms">
      Doar pentru abonamentul Individual. 4.99 EUR/lună după.
      <a href="#">Se aplică Termenii și condițiile.</a> Ofertă disponibilă doar
      pentru utilizatorii care nu au mai încercat versiunea Premium. Oferta se
      încheie pe 31.12.2022
    </p>
  </div>
</template>
<script>
export default {
  name: "FirstCard",
};
</script>
<style scoped>
.Card__container {
  box-shadow: 1px 1px 4px 1px rgb(143 141 141);
  padding: 10px 10px 10px 10px;
  border-radius: 5px;
  border: 2px rgb(51, 51, 51);
  margin: 10px 35px;
  background-color: white;
  width: 270px;
  height: 450px;
  text-align: left;
}

.Card__container span {
  background-color: #0d72ea;
  padding: 3px 7px;
  border-radius: 5px;
}

.Card__container h3 {
  display: block;
  font-size: 1.17em;
  margin-block-start: 1em;
  margin-block-end: 1em;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  font-weight: bold;
}

.Card__container p {
  font-size: 13px;
}

.Container__line {
  margin: 20px 10px 20px auto;
  border: 1px solid rgb(156, 156, 156);
  height: 0.8px;
}

.Content__container {
  display: flex;
}

.btn {
  margin: 80px 20px 20px 25px;
}

.Image__Container img {
  height: 15px;
  width: 12px;
  display: flex;
  padding: 5px;
}

.Description p {
  padding: 6px;
}

button {
  background-color: black;
  font-size: 13px;
  color: white;
  border: none;
  border-radius: 20px;
  padding: 10px 20px;
  text-align: center;
  width: 220px;
  margin: 40px 35px;
}

a {
  color: black;
}

#terms {
  margin-top: 20px;
}
</style>
