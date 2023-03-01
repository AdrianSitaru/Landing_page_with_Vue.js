<template>
  <div class="buttons">
    <button class="header-button1">{{btn1}}</button>
    <button class="header-button2">{{btn2}}</button>
  </div>
</template>

<script>
export default {

  data() {
    return {
      btn1: 'IA-ȚI 3 LUNI LA0.00 EUR',
      btn2: 'VEZI ABONAMENTELE'

    }
  },
  name: "TheButtons"
}
</script>

<style lang="scss">
.buttons {
  padding: 30px 0px;
  .header-button1 {
    background-color: black;
    text-align: center;
    color: white;
    width: 301px;
    height: 58px;
    border-radius: 30px;
    padding: 15px 65px;
    border: 1px solid black;
    margin: auto 25px 15px;
    cursor: pointer;
  }
  .header-button2 {
    background-color: #df0c8b;
    text-align: center;
    color: white;
    width: 301px;
    height: 58px;
    border-radius: 30px;
    padding: 15px 65px;
    border: 1px solid white;
    margin: auto 25px 15px;
    cursor: pointer;
  }
}

</style>