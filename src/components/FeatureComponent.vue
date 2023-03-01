<template>
  <div class="presentation-container">
      <img :src="data.image"/>
      <h3>{{ data.description1 }}</h3>
      <p>{{ data.description2 }}</p>
    </div>
</template>
<script>
export default ({
  name: 'FeatureComponent',
  props: ['data']
})
</script>
<style lang="scss">
.presentation-container {
  padding: 20px;
  img {
    margin-left: 20px;
    height: 120px;
  }
}

</style>