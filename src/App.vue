<template>
  <div>
    <Podcast :content= "podcast"  />  
    <Podcast :content= "podcast"  />  
    <Podcast :content= "podcast"  />  
    <Podcast :content= "podcast"  />  


  </div>
</template>

<script>
  import Podcast from "./components/Podcast.vue"
  
  export default{
    name: 'App',

  data() {
    return {
      podcast: {
        event_1: "DATA STRUCTURES",
        name_1: "Jacqueline Cardozo",
        profession_1: "Front-end Dev Leader",
        event_2: "TECH TO WATCH IN 2020",
        name_2: "João Olivio",
        profession_2: "Front-end Dev Leader",
        event_3: "HOW TO GET BETTER AT PROBLEM SOLVING",
        name_3: "Derrick Pierce",
        profession_3: "Front-end Dev Leader",
        event_4: "DATA STRUCTURES",
        name_4: "Jacqueline Cardozo",
        profession_4: "Front-end Dev Leader"
      }
    }
  }, 
      
    components: { 
      Podcast 
    } 
  }
</script>

<style>
  body{
    background: rgb(240, 240, 240);
  }
</style>
