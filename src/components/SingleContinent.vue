<template>
    <div :class="continent.country_name=='United States of America'? 'deepblue': 'blue'">
                        <h2> Continents, Countries & Capitals: {{continent.continent_name}}</h2>
                        <div2 :class="continent.country_name=='United States of America'? 'deepblue': 'blue'">
                        
                        <h4> Continent ID: {{continent.continent_id}}</h4>
                        <h4> Continent Name: {{continent.continent_name}}</h4>
                        <h4> Country ID: {{continent.country_id}}</h4>
                        <h4> Country Name: {{continent.country_name}}</h4>
                        <h4> Capital Name: {{continent.capital_name}}</h4></div2>
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

.deepblue{
    background-color: rgb(21, 54, 238);
    border: 1px solid rgb(2, 40, 255);
    color: white;
}

h4{  
    margin: 2px;
    text-align: left;
}

div{
    width: 80%;
    height: 300px;
    border: 1px solid rgb(255, 255, 255);
    background-color: rgb(255, 255, 255);
    color: black;
    font-family: 'Times New Roman', Times, serif;
    padding: 1em;
    text-align: center;
    margin: auto;
    position: relative;
}

div2{
      width: 90%;
      height: 60%;
      background-color: rgb(203, 211, 255);
      color: rgb(51, 51, 56);
      font-family: 'Times New Roman', Times, serif;
      font-size: 18px;
      letter-spacing: 2px;
      text-align: center;
      line-height: 250%;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }

.blue{
background-color: rgb(255, 255, 255) !important;
}
</style>
