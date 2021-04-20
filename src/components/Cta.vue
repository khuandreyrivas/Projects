<template>
  <div> 
    <a class="cta" href="/"><strong>VIEW MORE</strong></a> 
    <router-view></router-view>
  </div>
</template>

<script>
  export default {
    name:'Cta'
  }
</script>

<style scoped>
  .cta {
    position: absolute;
    top: 660px;
    left: 770px;
    width: 140px;
    height: 50px;
    border: 1px solid black;
    text-decoration: none;
    text-align: center;
    line-height: 3em;;
    color: #000;
  }
</style>