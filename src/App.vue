<template>
  <div id="app">
    <weather></weather>
  </div>
</template>

<script>
import weather from './components/weather'

export default {
  name: 'app',
  components: {
    weather
  }
}
</script>

<style>

  body {

    font-family: Roboto, Arial;
    font-size: 1.2em;
    color: #888;

  }
</style>
