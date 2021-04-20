<template>
  <div id="header">
    <h1>Last <span class="title">Episodes</span></h1>
  </div>

  <div id="navigation">
    <ul>
      <li><strong><a href="">NEW</a></strong></li>
      <li><strong><a href="">DEVELOPMENT</a></strong></li>
      <li><strong><a href="">DESIGN</a></strong></li>
      <li><strong><a href="">PROJECT MANAGEMENT</a></strong></li>
    </ul>
  </div>
</template>

<script>
  export default {
    name:'Header',
  }
</script>

<style scoped>
  #header>h1 {
    font-size: 85px;
    text-align: center;
    position: relative;
    right: 85px;
    top: 70px;
    text-decoration-line: underline;
    text-decoration-color: rgb(138, 235, 227);
  }

  .title {
    text-shadow: -90px -40px rgba(0, 0, 0, 0.2);
    text-decoration: none;
  }

  #navigation {
    position: absolute;
    left: 530px;
    top: 240px;
  }

  #navigation li {
    display: inline;
  }

  #navigation a {
    text-decoration: none;
    color: #000;
    font-size: 15px;
    margin: 15px;
  }
  
  #navigation a:hover {
    cursor: pointer;
  }

</style>