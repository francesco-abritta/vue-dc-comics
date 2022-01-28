<template>
  <div>
        <div class="link">
            <div class="elenchi">
                <div class="col1">
                    <ul class="ulFooter">
                        DC COMICS
                        <li v-for="(elemento, indice) in links1" :key="indice">{{elemento.text}}</li>
                    </ul>
                    <ul class="ulFooter">
                        SHOP
                        <li v-for="(elemento, indice) in links2" :key="indice">{{elemento.text}}</li>
                    </ul>
                </div>
                
                <div class="col2">
                    <ul class="ulFooter">
                        DC
                        <li v-for="(elemento, indice) in links3" :key="indice">{{elemento.text}}</li>
                    </ul>
                </div>

                <div class="col3">
                    <ul class="ulFooter">
                        SITES
                        <li v-for="(elemento, indice) in links4" :key="indice">{{elemento.text}}</li>
                    </ul>
                </div>
                    
            </div>
            <img src="../../../assets/img/dc-logo-bg.png" alt="">
        </div>
        
  </div>
</template>

<script>
export default {
    name: 'Link',
    data() {
      return{
        links1: [
          {
            text:'Characters'
          },
          {
            text:'Comics'
          },
          {
            text:'Movies'
          },
          {
            text:'TV'
          },
          {
            text:'Games'
          },
          {
            text:'Videos'
          },
          {
            text:'News'
          },
          
        ],
        links2: [
          {
            text:'Shop Dc'
          },
          {
            text:'Shop Dc Collectibiles'
          },
          
        ],
        links3: [
          {
            text:'Terms of use'
          },
          {
            text:'Privacy policy'
          },
          {
            text:'Ad choises'
          },
          {
            text:'Advertising'
          },
          {
            text:'Jobs'
          },
          {
            text:'Subscription'
          },
          {
            text:'Talent Workshop'
          },
          {
            text:'CPSC Certificates'
          },
          {
            text:'Ratings'
          },
          {
            text:'Shop Help'
          },
          {
            text:'Contact us'
          },
          
        ],
        links4: [
          {
            text:'DC'
          },
          {
            text:'MAD Magazine'
          },
          {
            text:'DC Kids'
          },
          {
            text:'DC Universe'
          },
          {
            text:'DC Power Visa'
          },
          
        ]
    }
  }
}
</script>

<style scoped>
  @import './Link.scss';
</style>