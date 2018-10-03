<template>
    <div id="app">
      <img class="center" alt="Vue logo" src="./assets/tnttlogo.png">
      <h1>Welcome to ADLNC TNTT!</h1>
      <orgchart/>
      <bch/>
  </div>
</template>

<script>
import orgchart from './components/orgchart.vue'
import bch from './components/bch.vue'

export default {
  name: 'app',
  components: {
    orgchart,
    bch
    }
}
</script>


<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
