<template>
  <div class="presentation-container">
    <div class="holder" v-for="(item, index) in items" :key="index" >
      <img :src="item.image">
      <h3>{{item.description1}}</h3>
      <p>{{item.description2}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "PresentationPart",
  data() {
    return {
      items: [
        {
          image: require('@/assets/presentation1.png'),
          description1: 'Descarci muzică.',
          description2: 'Asculți de oriunde.'
        },
        {
          image: require('@/assets/presentation2.png'),
          description1: 'Ascultă muzică fără anunțuri.',
          description2: 'Te bucuri non-stop de muzică.'
        },
        {
          image: require('@/assets/presentation3.png'),
          description1: 'Redă orice melodie.',
          description2: 'Chiar și pe dispozitivul mobil'
        },
        {
          image: require('@/assets/presentation4.png'),
          description1: 'Omiteri nelimitate.',
          description2: 'Doar apeși butonul Înainte.'
        }
      ]
    }
  }

}
</script>

<style>
.presentation-container {

  display: flex;
  justify-content: space-evenly;
}

.holder {
  margin: 30px 15px;
}
img {
  margin-left: 20px;
  height: 120px;
}

.holder h3 {
  padding: 10px;
}

.holder p {
  padding: 10px;
}



</style>