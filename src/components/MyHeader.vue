<template>
<div>
    <h1> {{continentName}} </h1>
    <h4> {{countryName}} </h4>
    <h4> {{capitalName}} </h4>
</div>
</template>

<script>

export default{ // Exporting Default Object
    name: 'MyHeader',
    props:{ 

        continentName:String,
        countryName:String,
        capitalName: String
    }
}

</script>

<style scoped>

div{
    text-align: center;
}

</style>
