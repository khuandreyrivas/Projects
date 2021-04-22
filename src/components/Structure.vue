<template>
  <div id="container">
    <div id="ball"></div>
      <Header />
      <PodcastOne />
      <PodcastTwo />
      <PodcastThree />
      <PodcastFour />
      <Cta />
  </div> 
</template>

<script>
   import Header from './Header.vue'
   import PodcastOne from './PodcastOne.vue'
   import Cta from './Cta.vue'
   import PodcastTwo from './PodcastTwo.vue'
   import PodcastThree from './PodcastThree.vue'
   import PodcastFour from './PodcastFour.vue'
   
   export default {
     name: 'Structure',
     
     components: {
       Header,
       Cta,
       PodcastOne,
       PodcastTwo,
       PodcastThree,
       PodcastFour,
     }, 

     props: {
      content: Object 
     }
   }
</script>

<style scoped>
  #container {
    background: white;
    position: absolute;
    top:0;
    left:0;
    width: 1800px;
    height: 100%;
  }
  
  #ball {
    width: 490px;
    height: 490px;
    background: rgb(138, 235, 227);
    border-radius: 245px;
    position: absolute;
    top: 50px;
    left: 200px;
  }    
</style>