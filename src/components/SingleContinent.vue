<template>
    <div :class="continent.country_name=='United States of America'? 'green': 'red'">
    <h2>{{continent.continent_name}}</h2>
                        <h4> {{continent.continent_id}}</h4>
                        <h4> {{continent.continent_name}}</h4>
                        <h4> {{continent.country_id}}</h4>
                        <h4> {{continent.country_name}}</h4>
                        <h4> {{continent.capital_name}}</h4>
    </div>
</template>

<script>
export default{
    name: 'SingleContinent',
    props: {
        continent: Array
    }
}
</script>

<style scoped>

.green{
    background-color: rgb(78, 240, 78);
}

h4{
    margin: 2px;
}

div{
    background-color: #ff672f;
    color: black;
    padding: 1em;
    text-align: center;
    width: 80%;
    margin: auto;
}

.red{
background-color: rgb(255, 204, 185) !important;
}
</style>