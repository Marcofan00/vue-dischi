<template>
 <div id="cards">
     <img :src="details.poster" alt="">
     <h2>{{details.title}}</h2>
     <span><p>{{details.author}}</p></span>
     <span><p>{{details.year}}</p></span>
 </div>
</template>

<script>
export default {
  name: 'Mycards',
  props:{
      details:Object,
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#cards{
    margin: 30px 15px 30px;
    background-color: rgb(38, 48, 58);
    height: auto;
    width: 13%;
    text-align: center;
    padding: 20px;
    
}
img{
    width: 100%;
}
h2 {
    color: white;  
}
p{
color: rgb(134, 132, 132); 
}
</style>