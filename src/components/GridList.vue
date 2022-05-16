<template>
    <section>
        <h2>{{title}}</h2>
       <ul>
        <card-component v-for="(card) in items" :key="card.id" :item="card" />
      </ul>
     
    </section>
</template>

<script>
import CardComponent from './CardComponent.vue'
//import {state, actions} from '../store.js'
export default {
  components: { CardComponent },
    name: 'GridList',
    props:{
        items: Array,
        loader: Boolean,
        title: String
    },//['items','loader'],
    data(){
        return {
            
        }
    },
    computed: {
        // mysearch(){
        //     return state.search
        // }
    },
    methods:{
        // leggi(){
        //     actions.setSearch('aaaaa')
        // }
    }
}
</script>

<style lang="scss">

</style>