<template>
	<div class="premium-card">
    <span>3 Luni Gratuite</span>
    <h3>{{ data.title }}</h3>
    <p>{{ data.price }}</p>
    <div class="Content__container">
      <div class="Image__Container">
        <img src="../assets/tick.png" alt="image" />
        <img src="../assets/tick.png" alt="image" />
        <img src="../assets/tick.png" alt="image" />
      </div>
      <div class="Description"
           v-for="(option, index) in data.options"
           :key="index">
        <p>{{ option }}</p>
      </div>
    </div>
	</div>
</template>

<script>
	export default {
		name: 'PremiumCard',
    props: {
      data: Object
    }
	}
</script>

<style lang="scss">
	.premium-card {
	}
</style>
