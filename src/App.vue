<template>
    <div class="background">
      <Navbar />
      <Card />
      <Next />
    </div>
    <div id="models">
      <Models />
    </div>
</template>

<script>
import './assets/main.css'
import Navbar from './components/Navbar.vue'
import Card from './components/Card.vue'
import Next from './components/Next.vue'
import Models from './components/Models.vue'


export default {
  name: 'App',
  components: {
    Navbar, 
    Card,
    Next,
    Models
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.background {
  background-image: url('./assets/background.png');
  height: 100vh;
  background-color: rgba(0, 0, 0, 0.8);
  background-position: center center;
}

#models {
  overflow: auto;
  width: 100%;
  height: 100vh;
  background-image: url('./assets/model2.png');
  background-color: rgba(0, 0, 0, 0.7);
  background-position: center center;
}
</style>
