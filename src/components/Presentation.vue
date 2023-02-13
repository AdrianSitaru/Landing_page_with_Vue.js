<template>
  <div class="PremiumSection">
    <h2>De ce să treci la Premium?</h2>
    <div class="Container">
      <div>
        <img src="../assets/1.png" alt="image" />
        <h3>Descarci muzică.</h3>
        <p>Asculți de oriunde.</p>
      </div>
      <div>
        <img src="../assets/2.png" alt="image" />
        <h3>Ascultă muzică fără anunțuri.</h3>
        <p>Te bucuri non-stop de muzică.</p>
      </div>
      <div>
        <img src="../assets/3.png" alt="image" />
        <h3>Redă orice melodie.</h3>
        <p>Chiar și pe dispozitivul mobil</p>
      </div>
      <div>
        <img src="../assets/4.png" alt="image" />
        <h3>Omiteri nelimitate.</h3>
        <p>Doar apeși butonul Înainte.</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "PresentationSection",
};
</script>
<style>
.PremiumSection {
  display: block;
  background-color: white;
  text-align: center;
}
.PremiumSection h2 {
  font-size: 42px;
}

.Container {
  margin: 25px 60px;
  display: flex;
  justify-content: space-between;
}

.Container h3 {
  padding: 10px;
}

.PremiumSection .Container img {
  width: 90px;
  height: 90px;
}
</style>
