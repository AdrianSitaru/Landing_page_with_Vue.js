<template>

  <div class="feature-component">
    <div class="feature-content">
      <img :src="data.image"/>
      <h3>{{ data.description1 }}</h3>
      <p>{{ data.description2 }}</p>
    </div>
  </div>
</template>
<script>
export default ({
  name: 'FeatureComponent',
  props: ['data'],
})
</script>
<style lang="scss">
.feature-component {
  height: 300px;
  align-items: center;
  display: flex;

  @media (min-width: 0) {
    padding: 10px;
    img {
      padding: 10px;
      margin-left: 10px;
      height: 120px;
    }
  }
}
</style>