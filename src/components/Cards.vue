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
        'price': 29.99,
        'imgUrl': 'https://neurosciencenews.com/files/2023/06/coffee-brain-caffeine-neuroscincces.jpg',
        'addedOn': '2020-01-02',
        'likes': 3
      },
      {
        'id': 2,
        'title': 'Battlecreek Yirgacheffee',
        'price': 29.99,
        'imgUrl': 'https://insanelygoodrecipes.com/wp-content/uploads/2020/07/Cup-Of-Creamy-Coffee-500x375.png',
        'addedOn': '2020-01-05',
        'likes': 2
      },
      {
        'id': 3,
        'title': 'Primo Passo',
        'price': 29.99,
        'imgUrl': 'https://img.freepik.com/free-photo/fresh-coffee-steams-wooden-table-close-up-generative-ai_188544-8923.jpg',
        'addedOn': '2020-01-05',
        'likes': 5
      },
      {
        'id': 4,
        'title': 'Little Nap Brazil',
        'price': 29.99,
        'imgUrl': 'https://images.summitmedia-digital.com/spotph/images/2022/09/28/coffee-1-1-1664301131.jpg',
        'addedOn': '2020-01-06',
        'likes': 332
      },
      {
        'id': 5,
        'title': 'Little Nap Blend',
        'price': 29.99,
        'imgUrl': 'https://tracextech.com/wp-content/uploads/2022/02/coffee-traceability-solution.jpeg',
        'addedOn': '2020-01-07',
        'likes': 0
      },
      {
        'id': 6,
        'title': 'French Truck Peru Cajamarca',
        'price': 29.99,
        'imgUrl': 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSTeQu2f_5Y1z8Tu-xsA9X8oSD18xyingfMXA&usqp=CAU',
        'addedOn': '2020-01-08',
        'likes': 1
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
