<template>
     <li>
          id: {{item.id}}<br />
          titolo originale: {{item.original_title ? item.original_title : item.original_name}}<br />
          titolo: {{item.title ? item.title : item.name}}<br />
          lingua: {{item.original_language}}<br />
         
          voto: {{item.vote_average}}<br />
        </li>
</template>

<script>
export default {
    name:'CardComponent',
    props: ['item']
    
}
</script>

<style lang="scss">

</style>