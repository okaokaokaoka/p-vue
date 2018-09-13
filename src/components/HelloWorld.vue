<template>
  <div class="hello">
    <img src="../assets/logo.png" class="vue-logo">
    <h1>{{ msg }}</h1>
    <router-link to="/about">
      <v-btn>岡田徹について知る</v-btn>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Vueを使ってみようや'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  margin-top: 30px;
}
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  text-decoration: none;
}
</style>
