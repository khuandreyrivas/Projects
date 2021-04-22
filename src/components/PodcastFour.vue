<template>
  <!--This is podcast 4 card scope-->
  <div class="podcast_4" v-show="!displayPodcast">
    <div class="podcast_structure">
      <h1>DATA STRUCTURES</h1>
      <h3>Jacqueline Cardozo</h3>
      <h3 class="profession">Front-end Dev Leader</h3>
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
</template>

<script>
export default {
  name: 'PodcastFour'
}
</script>

<style scoped>
  .podcast_4 {
    position: absolute; 
    top: 300px;
    left: 1092px;
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

  .profession {
    color:rgba(0, 0, 0, 0.4);
  }
</style>