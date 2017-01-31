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

  * {
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    border: 1px solid #999;
  }

  body {

    font-family: Roboto, Arial;
    font-size: 1.2em;
    color: #888;

  }
</style>
