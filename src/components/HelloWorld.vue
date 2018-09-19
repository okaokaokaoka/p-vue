<template>
  <div class="hello">
    <!-- <Carousel/> -->
    <h1>{{ msg }}</h1>
    <router-link to="/about">
      <v-btn large color="white">About</v-btn>
    </router-link>
    <router-link to="/portfolio">
      <v-btn large color="white">Works</v-btn>
    </router-link>
    <router-link to="/contact">
      <v-btn large color="white">Contact</v-btn>
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
      msg: 'Hello World!'
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
