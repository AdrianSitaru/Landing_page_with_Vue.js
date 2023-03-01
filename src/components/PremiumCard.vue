<template>
  <div>
    <div class="card-holder">
      <span>{{ cardData.span }}</span>
      <h4>{{ cardData.title }}</h4>
      <p class="price">{{ cardData.paragraph }}</p>
      <div class="card-line"></div>
      <ul>
        <li v-for="item in cardData.list" :key="item">
          <img :src="item.image" alt="image"/>
          <span class="list-description"> {{ item.description }} </span>
        </li>
      </ul>
      <button class="card-button">{{ cardData.button }}</button>
      <p class="card-terms">{{ cardData.terms }}</p>
    </div>
  </div>
</template>
<script>
export default {
  name: "ThePremiumCard",
  props: {
    cardData: {
      type: Object,
    }
  },
}
</script>
<style lang="scss">


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

  span {
    font-size: 15px;
    margin: 10px 0px;
  }

  ul {
    height: 180px;
  }

  li {
    list-style: none;
    display: flex;
  }

  img {
    margin: 10px;
    display: block;
    width: 19px;
    height: 20px;
  }

  h4 {
    font-size: 20px;
    padding: 5px 0px;

  }

  .content-holder {
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

  .list-description {
    background-color: white;
    margin-top: 5px;
  }

  span {
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
}
</style>