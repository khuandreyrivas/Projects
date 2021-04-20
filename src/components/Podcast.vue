<template>

    <div id="container">
      <div id="ball"></div>

      <Header />

    <!--This is podcast 1 card scope-->
     <div class="podcast_1">
        <div class="podcast_structure">
          <h1>{{content.event_1}}</h1>
          <h3>{{content.name_1}}</h3>
          <h3 class="profession">{{content.profession_1}}</h3>
          <!--This is the play button for the podcast-->
          <button>
            <i class="material-icons" >play_circle_filled</i>
          </button> 
          <!--This is the icon indicating the podcast duration-->
          <div class="clock">
            <i class="material-icons">query_builder</i>
            <span class="time">1h 20m</span>
          </div>
        </div>
      </div>
      <!--This is podcast 2 card scope-->
      <div class="podcast_2">
        <div class="podcast_structure">
          <h1> {{content.event_2}} </h1>
          <h3>{{content.name_2}}</h3>
          <h3 class="profession"> {{content.profession_2}} </h3>
          <!--This is the play button for the podcast 2-->
          <button>
            <i class="material-icons">play_circle_filled</i>
          </button> 
          <!--This is the icon indicating the podcast duration-->
          <div class="clock">
            <i class="material-icons">query_builder</i>
            <span class="time">1h 20m</span>
          </div>
        </div>
      </div>
      <!--This is podcast 3 card scope-->
      <div class="podcast_3">
        <div class="podcast_structure">
          <h1> {{content.event_3}} </h1>
          <h3>{{content.name_3}}</h3>
          <h3 class="profession"> {{content.profession_3}} </h3>
          <!--This is the play button for the podcast 3-->
          <button>
            <i class="material-icons">play_circle_filled</i>
          </button> 
          <!--This is the icon indicating the podcast duration-->
          <div class="clock">
            <i class="material-icons">query_builder</i>
            <span class="time">1h 20m</span>
          </div>
        </div>
      </div>  
      <!--This is podcast 4 card scope-->
      <div class="podcast_4">
        <div class="podcast_structure">
          <h1> {{content.event_4}} </h1>
          <h3> {{content.name_4}} </h3>
          <h3 class="profession"> {{content.profession_4}} </h3>
          <!--This is the play button for the podcast 4-->
          <button>
            <i class="material-icons">play_circle_filled</i>
          </button> 
          <!--This is the icon indicating the podcast duration-->
          <div class="clock">
            <i class="material-icons">query_builder</i>
            <span class="time">1h 20m</span>
          </div>
        </div>
      </div>         
     
      <Cta />

    </div> 

</template>

<script>
   import Header from './Header.vue'
   import Cta from './Cta.vue'
   export default {
     name: 'Podcast',
     
     components: {
       Header,
       Cta,
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
  
  .podcast_structure{
      background:#fff;
      border: 1px solid black;
      font-family: sans-serif;
      width: 250px;
      height: 320px;
      display: inline-block;
      text-align: center;
      margin: 6px;
  }

  .podcast_structure:hover{
     box-shadow: -8px -10px 15px rgba(0, 0, 0, 0.2);

  }

  div h1 {
    font-size: 30px;
  }

  button {
    background: none;
    border: none;
    position:absolute;
    left: 35px;
    top: 275px;
  }

  button:hover {
    background: rgb(211, 234, 235);
    cursor: pointer;
  }
  .material-icons { 
    font-size: 36px;
    }

  .clock {
    position:absolute;
    left: 150px;
    top: 275px; 
  }

  span.time {
    position: absolute;
    top: 5px;
  }

 .podcast_1 {
    position: absolute; 
    top: 300px;
    left: 300px;
  }

  .profession {
    color:rgba(0, 0, 0, 0.4);
  }

  .podcast_2 {
    position: absolute; 
    top: 300px;
    left: 564px;
  }

  .podcast_3 {
    position: absolute; 
    top: 300px;
    left: 828px;
  }

  .podcast_4 {
    position: absolute; 
    top: 300px;
    left: 1092px;
  }
  
</style>