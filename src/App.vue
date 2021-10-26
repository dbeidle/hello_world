<template>
  <div id="app" class="container">
    <h1 @click="onClick">HELLO WORLD!</h1>
    
    <VideoView />
        <p>This video is owned and copyrighted by <a href="https://www.capitolrecords.com/#/">Capitol Records</a></p>

    <div>
      <p>Powered by:</p>
    <img class="image" src="vue_logo.png" alt="Vue JS Logo"/></div>
  </div>
</template>

<script>
  import VideoView from "./components/VideoView.vue"
  
  export default {
    name: "App",
    components: {
    
      VideoView
    },
    methods: {
      onClick() {
        alert("HELLO WORLD!")
      }
    }
  };
</script>

<style>
  body {
    background-color: slategrey;
  }
  #app {
    color: #fff;
  }

  h1 {
    display:flex; 
    justify-content:center;
    align-items:center; 
    padding: 20px;
    cursor: pointer;
  }
  p {
     
      text-align: center; 
  }
  .image {
    display: block;
    margin: auto;
    height: 15%;
    width: 15%;
  }
  a {
    color: white;
    text-decoration: none;
  }
</style>
