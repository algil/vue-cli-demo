<template>
  <div id="app">
    <p>BaseUrl: {{baseUrl}}</p>
    <svg class="icon">
      <use :xlink:href="`${baseUrl}icons.svg#menu`"></use>
    </svg>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      baseUrl: process.env.BASE_URL
    }
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.icon {
  border: 1px solid orange;
  display: inline-block;
  fill: red;
  height: 3.2rem;
  stroke: blue;
  stroke-linecap: round;
  stroke-linejoin: round;
  stroke-width: .2rem;
  width: 3.2rem;
}
</style>
