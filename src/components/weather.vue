<template>
  <div class="weather">

    <div class="location">{{location}}</div>
    <div class="date">{{date}}</div>
    <div class="description">{{description}}</div>
    <div class="current">
      <div class="visual">
        <div class="cloud">cloud</div>
        <div class="temp">{{temp}}</div>
        <div class="scale">º</div>
      </div>
      <div class="text">
        <div class="precipitation">Precipitation: {{precipitation}}</div>
        <div class="humidity">humidity: {{humidity}}</div>
        <div class="wind">wind: {{wind}}</div>
        <div class="pollen">pollen: {{pollen}}</div>
      </div>
    </div>
    <div class="forecast">
      <div class="forecast-day" v-for="forecast in forecasts">
        <div class="date">{{forecast.date}}</div>
        <div class="date">{{forecast.icon}}</div>
        <div class="high-temp">{{forecast.hightemp}}</div>
        <div class="low-temp">{{forecast.lowtemp}}</div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'weather',
  data () {
    return {
      location: 'NY City',
      date: 'Tursday 36 apa',
      description: 'Desc here',
      temp: 25,
      precipitation: '100%',
      humidity: '97%',
      wind: '4mph SW',
      pollen: 36,
      forecasts: [
        {'date': 'Monday', 'icon': 'cloud', 'lowtemp': 28, 'hightemp': 45},
        {'date': 'Tuesday', 'icon': 'sun', 'lowtemp': 28, 'hightemp': 45},
        {'date': 'Wednesday', 'icon': 'sun-cloud', 'lowtemp': 28, 'hightemp': 45},
        {'date': 'Thursday', 'icon': 'raining', 'lowtemp': 28, 'hightemp': 45},
        {'date': 'Friday', 'icon': 'raining', 'lowtemp': 28, 'hightemp': 45},
        {'date': 'Saturday', 'icon': 'raining', 'lowtemp': 28, 'hightemp': 45},
        {'date': 'Sunday', 'icon': 'raining', 'lowemp': 28, 'hightemp': 45}
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
