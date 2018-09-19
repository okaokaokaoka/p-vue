<template>
  <div class="about">
    <v-container>
      <div class="mt-3">
        <p class="display-1">
          My history.
        </p>
      </div>
      <div class="mt-3 desc-wrapper">
          <p class="text-sm-left text-md-center">Mar.2014: さいたま市立浦和高校卒業</p>
          <p class="text-sm-left text-md-center">Apr.2014: 大阪大学経済学部入学</p>
          <p class="text-sm-left text-md-center">Aug.2016: Web制作を開始</p>
          <p class="text-sm-left text-md-center">Sep.2017: 大規模ビジネスコンテストにて優勝</p>
          <p class="text-sm-left text-md-center">Mar.2018: Bullzにて、自社サービス開発</p>
      </div>
      <div class="mt-5">
        <p class="display-1">
          Skills.
        </p>
      </div>
      <div class="mt-3 skills-wrapper">
        <p>HTML, CSS(Sass), jQuery</p>
        <p>Ruby, Ruby on Rails</p>
        <p>React.js, Vue.js</p>
        <p>Others: Firebase, Heroku, ドメイン設定, WordPressサイト構築, スクレイピング(Python)</p>
      </div>
    </v-container>
  </div>
</template>

<script>
import Card from './components/contents/Card'

export default {
  components: {
    Card
  }
}
</script>

<style scoped>
.desc-wrapper p {
  font-size: 18px;
  text-align: center;
}
.skills-wrapper p {
  font-size: 18px;
  text-align: center;
}
@media (max-width: 480px) {
  .desc-wrapper p {
    font-size: 16px;
    text-align: left;
  }
}
@media (max-width: 480px) {
  .skills-wrapper p {
    font-size: 18px;
    text-align: left;
  }
}
</style>
