<template>
  <div class="hello">
    <div class="mt-5">
      <img src="../assets/profile_pic.jpg" alt="profile" height="200px">
    </div>
    <div class="mb-5 mt-3">
      <h1>Toru Okada(22)</h1>
      <h2 color="grey lighten-3">岡田 徹</h2>
      <div class="mt-1 intro-wrapper">
        <span>1996年生まれ東京都在住、webエンジニア。</span><br>
        <span>0→1のサービス立ち上げに強みを持つ。</span><br>
        <span>幼少期よりサイトなど経験。</span><br>
        <span>大阪大学の4年目を休学中</span>
      </div>
    </div>
    <!-- <div class="mt-2 mb-4">
      <a href="https://twitter.com/okaokatoru">
        <img src="../assets/twitter.png" alt="twitter" width="50px">
      </a>
      <a href="https://www.facebook.com/okyaokya.yanen">
        <img src="../assets/facebook.png" alt="facebook" width="50px">
      </a>
      <a href="https://github.com/okaokaokaoka">
        <img src="../assets/git.png" alt="github" width="50px">
      </a>
    </div> -->
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
    }
  },
  methods: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  margin-bottom: 30px;
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

.intro-wrapper {
  font-size: 16px;
}

@media (max-width: 480px) {
  .intro-wrapper {
    font-size: 14px;
  }
}
</style>
