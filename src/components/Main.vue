<template>

    <div>
          <div class="card" v-for="card in cards" :key="card.id">
              <Card :title= card.title  :description= card.description />
            </div>
    </div>

</template>

<script>
import Card from "./Card.vue"

export default {
    components: {
        Card,

    },
   
  data() {
     return {
        cards: [ {
           "id": 1, 
           "title": "Title-1",
           "description": "this is blog entry-1",
           
        },
        {
           "id": 2, 
           "title": "Title-2",
           "description": "this is blog entry-2",
           
        }, 
        {
           "id": 3, 
           "title": "Title-3",
           "description": "this is blog entry-3",
          
        },
       ]
    }
    },
}
</script>

<style>

</style>