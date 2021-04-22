<template>
  <div>
    <Structure  />   
  </div>
</template>

<script>
  import Structure from "./components/Structure.vue"
  
  export default{
    name: 'App',
      
    components: { 
      Structure 
    } 
  }
</script>

<style>
  body{
    background: rgb(240, 240, 240);
  }
</style>
