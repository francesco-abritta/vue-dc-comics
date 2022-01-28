<template>
  <div>
        <div class="sezione">
            <button><a href="#"><strong>SIGN-UP NOW</strong></a></button>
            <div class="social">
                <ul class="ulFooter3">
                    <strong>FOLLOW US</strong>
                    <li :key="indice" v-for="(elemento, indice) in social"><img :src="elemento.image" alt=""></li>
                </ul>
            </div>
        </div>
  </div>
</template>

<script>
export default {
    name: 'Social',
    data() {
      return{
        social: [
          {
            image: require("../../../assets/img/footer-facebook.png"),
          },
          {
            image: require("../../../assets/img/footer-periscope.png"),
          },
          {
            image: require("../../../assets/img/footer-pinterest.png"),
          },
          {
            image: require("../../../assets/img/footer-twitter.png"),
          },
          {
            image: require("../../../assets/img/footer-youtube.png"),
          },
        ]
      }
    }
}
</script>

<style scoped>
  @import './Social.scss';
</style>