<template>
  <div class="feature-component">
    <div>
      <img :src="data.image"/>
      <h3>{{ data.description1 }}</h3>
      <p>{{ data.description2 }}</p>
    </div>
  </div>
</template>
<script>
export default ({
  name: 'FeatureComponent',
  props: ['data']
})
</script>
<style lang="scss">
.feature-component {
  padding: 10px;

  img {
    padding: 10px;
    margin-left: 10px;
    height: 100px;
  }
}
</style>