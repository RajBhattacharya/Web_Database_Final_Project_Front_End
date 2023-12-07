<template>
   

    <div v-for="continent of continents" :key="continent._id" >
       <SingleContinent :continent=continent />
    </div>
</template>

<script>
import SingleContinent from './SingleContinent.vue'

export default{
    name: 'ContinentBox',
    props:{
        continents: Array
    },
    components:{
        SingleContinent
    }
}

</script>

<style scoped>
div{

background-color: rgb(255, 125, 125);
    color: black;
    padding: 1em;
    text-align: center;
    width: 80%;
    margin: auto;
}
</style>