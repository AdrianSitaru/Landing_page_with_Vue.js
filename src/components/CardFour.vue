<template>
  <div class="Card__container">
    <span>O Luna Gratuit</span>
    <h3>Student</h3>
    <p>2.49 EUR/lună după perioada ofertei Un cont</p>
    <div class="Container__line"></div>
    <div class="Content__container">
      <div class="Image__Container">
        <img src="../assets/tick.png" alt="image" />
        <img src="../assets/tick.png" alt="image" />
        <img src="../assets/tick.png" alt="image" />
        <img src="../assets/tick.png" alt="image" />
      </div>
      <div class="Description">
        <p>
          Reducere specială pentru studenții eligibili care urmează cursurile
          unei universități
        </p>
        <p>Ascultă muzică fără anunțuri</p>
        <p id="Paragraph">Redai de oriunde chiar și offline</p>
        <p id="Paragraph">Redare la cerere</p>
      </div>
    </div>
    <button>SĂ ÎNCEPEM</button>
    <p id="terms">
      Se aplică <a href="#">Termenii și condițiile.</a> Luna gratuită nu este
      disponibilă utilizatorilor care au încercat deja versiunea Premium.
    </p>
  </div>
</template>
<script>
export default {
  name: "CardFour",
};
</script>
<style>
#Paragraph {
  margin-top: 10px;
}
</style>
