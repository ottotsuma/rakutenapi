<template>
  <div id="app">
    <h1>Welocome to the Most Funny Meme Application</h1>
    <meme />
    <jokes />
  </div>
</template>

<script>
import Meme from "./components/Meme"
import Jokes from "./components/Jokes"

export default {
  name: 'App',
  components: {
    meme: Meme,
    jokes: Jokes
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
