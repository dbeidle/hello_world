<template>
  <div id="app" class="container">
    <h1 @click="onClick">HELLO WORLD!</h1>
    
    <VideoView />
    
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
}
</style>
