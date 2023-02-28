<template>
  <div>
    <div class="card-holder">
      <span>{{ cardData.span }}</span>
      <h4>{{ cardData.title }}</h4>
      <p class="price">{{ cardData.paragraph }}</p>
      <div class="card-line"></div>
      <div class="content-holder">
        <div class="image-holder">
          <img v-bind:key="images.id" v-for="images in cardData.images" :src="images" alt="image">
        </div>
        <div >
          <p v-bind:key="description.id" v-for="description in cardData.description" class="description-holder">{{ description }}</p>
        </div>
      </div>
      <button class="card-button">{{ cardData.button }}</button>
      <p class="card-terms">{{ cardData.terms }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "ThePremiumCard",
  props: {
    cardData: Object
  },


}

</script>

<style>
span {
  font-size: 15px;
}
img {
  margin: 10px;
  display: block;
}

.card-holder h4 {
  font-size: 20px;
  padding: 5px 0px;

}

.content-holder{
  display: flex;
  height: 230px;
}
.price {
  font-size: 17px;
  margin-top: 5px;
}

.description-holder {
  font-size: 15px;
  display: block;
  padding-top: 10px;

}
.card-holder {
  box-shadow: 1px 1px 4px 1px rgb(143 141 141);
  padding: 10px 10px 10px 10px;
  border-radius: 5px;
  border: 2px rgb(51, 51, 51);
  margin: 10px 35px;
  background-color: white;
  width: 270px;
  height: 550px;
  text-align: left;
}

.card-holder span {
  background-color: #0d72ea;
  padding: 3px 7px;
  border-radius: 5px;
}
.card-line {
  margin: 20px 10px 20px auto;
  border: 1px solid rgb(156, 156, 156);
  height: 0.8px;
}

.image-holder img {
  height: 19px;
  width: 17px;
  padding: 5px;

}

.card-terms {
  font-size: 12px;
}

.card-button {
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
</style>