<template>
  <div class="Card__container">
    <span>O Luna Gratuit</span>
    <h3>Duo</h3>
    <p>6.49 EUR/lună după perioada ofertei 2 conturi</p>
    <div class="Container__line"></div>
    <div class="Content__container">
      <div class="Image__Container">
        <img src="../assets/tick.png" alt="image" />
        <img src="../assets/tick.png" alt="image" />
      </div>
      <div class="Description">
        <p>2 conturi Premium pentru un cuplu care locuiește împreună</p>
        <p>Asculți muzică fără anunțuri, redai offline și la cerere</p>
      </div>
    </div>
    <button class="btn">SĂ ÎNCEPEM</button>
    <p id="terms">
      Se aplică <a href="#"> Termenii și condițiile.</a> Luna gratuită nu este
      disponibilăutilizatorilor care au încercat deja versiunea Premium.
    </p>
  </div>
</template>
<script>
export default {
  name: "SecondCard",
};
</script>
<style>
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
  padding: 10px;
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
