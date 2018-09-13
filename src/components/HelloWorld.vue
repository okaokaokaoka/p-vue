<template>
  <div class="hello">
    <img src="../assets/profile.jpg" class="profile-logo" height="300px">
    <h1>{{ msg }}</h1>
    <p>※この画像は高校生の頃のものであり実物とは異なります。</p>
    <router-link to="/about">
      <v-btn>岡田徹について知る</v-btn>
    </router-link>
    <router-link to="/portfolio">
      <v-btn>仕方ねえからポートフォリオを見てやるか…</v-btn>
    </router-link>
    <router-link to="/contact">
      <v-btn>儲かる話はこちら</v-btn>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'おかおかちゃん⭐'
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
.profile-logo {
  margin-top: 30px;
}
</style>
