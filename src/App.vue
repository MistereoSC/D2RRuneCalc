<template>
  <img class="mainbg" alt="Background" src="./assets/background.jpg">
  <Main/>
</template>

<script>
import Main from './Views/Main.vue'


export default {
  name: 'App',
  components: {
    Main,
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700;900&display=swap');

body {
  margin: 0;
  font-family: 'Roboto', sans-serif;
}

#app {
  font-family: 'Roboto', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.mainbg {
  width: 100%;
  height: 100%;
  position: fixed;
  top: 0;
  left: 0;
  transform: scaleX(-1);
  filter: brightness(1.2);
  z-index: -1;
}
</style>
