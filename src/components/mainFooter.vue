<template>
  <footer>
      <div class="bg-blue">
          <div class="container">
            <CardsDC v-for="(card, index) in cards" :key="index"
                :img="getImgUrl(card.src)"
                :imgAlt="card.text"
                :cardText="card.text"
             />
          </div>
      </div>
      <div class="container">
          nice footer
      </div>

  </footer>
</template>

<script>
import CardsDC from './CardsDC.vue'

export default {
    name: 'mainFooter',
    components: {
    CardsDC
    },
    data () {
        return {
            cards: [
                {
                    src: 'buy-comics-digital-comics.png',
                    text: 'Digital Comics'
                },
                {
                    src: 'buy-comics-merchandise.png',
                    text: 'Dc merchandise'
                },
                {
                    src: 'buy-comics-shop-locator.png',
                    text: 'subscription'
                },
                {
                    src: 'buy-comics-subscriptions.png',
                    text: 'comic shop locator'
                },
                {
                    src: 'buy-dc-power-visa.png',
                    text: 'dc power visa'
                }
            ]
        }
    },
    methods: {
      getImgUrl () {
        return require('../assets/img/' + `buy-comics-digital-comics.png`);
      }
    }
}
</script>

<style lang="scss" scoped>
  @import "../assets/styles/main";
  footer {

      .bg-blue {
          background-color: $mainColor;
          height: 100%;
          .container {
              display: flex;
              min-height: 20vh;
              gap: 1rem;
              flex-wrap: wrap;
              justify-content: space-between;
          }
      }
  }

</style>
