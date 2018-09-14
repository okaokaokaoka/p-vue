<template>
  <div class="hello">
    <!-- <Carousel/> -->
    <Parallax/>
    <h1>{{ msg }}</h1>
    <v-btn
      @click="coutnUp()"
      type="button"
      value="+1"
    >数字が増えるかもしれないよ</v-btn>
    <p>{{count}}</p>
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
import Carousel from './contents/Carousel'
import Parallax from './contents/Parallax'

export default {
  name: 'HelloWorld',
  components: {
    Carousel,
    Parallax
  },
  data () {
    return {
      msg: 'おかおかちゃん⭐',
      count: 0
    }
  },
  methods: {
    coutnUp () {
      this.count++
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* .hello {
  margin-top: 30px;
} */
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
