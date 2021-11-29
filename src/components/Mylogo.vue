<template>
 <div id="logo">
    <div class="logospotify"> 
        <img id="logospotify" src="../../src/assets/logo.spotify.png" alt="logo">
    </div> 
 </div>
</template>

<script>
export default {
  name: 'Mylogo',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#logo{
    background-color: rgb(38, 48, 58);
    height: 70px;
    display: flex;
    align-items: center;
}
#logospotify{
    width: 80px;
    height: 60px;
}
</style>