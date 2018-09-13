<template>
  <div id="app">
    <HeaderItem/>
    <img src="./assets/logo.png" class="vue-logo">
    <router-view/>
  </div>
</template>

<script>
import HeaderItem from './components/HeaderItem'

export default {
  name: 'App',
  components: {
    HeaderItem
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
  /* margin-top: 60px; */
}
.vue-logo {
  margin-top: 30px;
}
</style>
