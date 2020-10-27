<template>
  <div id="main">
      <StrokeMorph></StrokeMorph>
  </div>
</template>

<script>
// import StrokeAnimation from "./components/StrokeAnimation"
import StrokeMorph from "./components/CodeMorph"

export default {
  name: 'App',
  components: {
    StrokeMorph
  }
}
</script>

<style>
:root {
    --main-color: #1F3353;
    --compliment-color: #ffffff;
}

* {
    margin: 0;
    padding: 0;
}

#main {
    width: 100vw;
    height: 100vh;
    background-color: var(--main-color);
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
