<template>
  <MonthPanels />
</template>

<script>

import MonthPanels from './components/MonthPanels.vue'

export default {
  name: 'App',
  components: {
    MonthPanels
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
  margin-top: 40px;
}
</style>
