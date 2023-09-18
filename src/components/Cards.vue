<template>

  <div class="cards">

    <Card v-bind="card" v-for="card in cards" :key="card.id" />

  </div>

</template>

<script>

import Card from './Card'

export default {

  data: () => ({

    cards: [
      {
        'id': 1,
        'title': 'Battlecreek Columbia Coldono',
        'imgUrl': '/img/battlecreek-coffee-roasters-_1wDmr4dtuk-unsplash.jpg',
        'addedOn': '2020-01-02'
      },
      {
        'id': 2,
        'title': 'Battlecreek Yirgacheffee',
        'imgUrl': '/img/battlecreek-coffee-roasters-HvzR2yXtii4-unsplash.jpg',
        'addedOn': '2020-01-05'
      },
      {
        'id': 3,
        'title': 'Primo Passo',
        'imgUrl': '/img/jon-tyson-KRedbshBxEk-unsplash.jpg',
        'addedOn': '2020-01-05'
      },
      {
        'id': 4,
        'title': 'Little Nap Brazil',
        'imgUrl': '/img/lex-sirikiat-QouiCn7u6kw-unsplash.jpg',
        'addedOn': '2020-01-06'
      },
      {
        'id': 5,
        'title': 'Little Nap Blend',
        'imgUrl': '/img/manki-kim-mv7kxYh5Rko-unsplash.jpg',
        'addedOn': '2020-01-07'
      },
      {
        'id': 6,
        'title': 'French Truck Peru Cajamarca',
        'imgUrl': '/img/ryan-spaulding-_uncFvtOC-4-unsplash.jpg',
        'addedOn': '2020-01-08'
      }
    ]

  }),

  components: { Card }

}

</script>

<style scoped>

.cards {

  display: flex;

  justify-content: space-between;

  flex-wrap: wrap;

}

</style>
