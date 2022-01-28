<template>
  <div>
      <div class="merc">
          <section v-for="(elemento, indice) in merchandise" :key="indice">
            <img :src="elemento.image">
            <div>{{elemento.text}}</div>
          </section>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Merchandise',
    data() {
      return{
        merchandise: [
          {
            image: require("../../../assets/img/buy-comics-digital-comics.png"),
            text: 'DIGITAL COMICS'
          },
          {
            image: require("../../../assets/img/buy-comics-merchandise.png"),
            text: 'DC MERCHANDISE'
          },
          {
            image: require("../../../assets/img/buy-comics-shop-locator.png"),
            text: 'SUBSCRIPTION'
          },
          {
            image: require("../../../assets/img/buy-comics-subscriptions.png"),
            text: 'COMIC SHOP LOCATOR'
          },
          {
            image: require("../../../assets/img/buy-dc-power-visa.svg"),
            text: 'DC POWER VISA'
          },
        ]
    }
  }
}
</script>

<style scoped>
  @import './merchandise.scss';
</style>