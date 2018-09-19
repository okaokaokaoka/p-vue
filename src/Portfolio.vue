<template>
  <div class="portfolio">
  <v-container>
    <div class="mb-2">
      <h1>My Works.</h1>
    </div>
    <v-layout row wrap>
      <v-flex xs12 sm6 offset-sm3>
        <v-card class="mb-3">
          <img
            src="./assets/bullz-cp.png"
            width="100%"
          >
          <v-card-title primary-title class="justify-center">
            <div>
              <div class="headline">Bullzコーポレートサイト</div>
              <span class="grey--text">株式会社ブルズのコーポレートサイトを改修しました。</span>
            </div>
          </v-card-title>

          <v-card-actions>
            <v-btn flat color="purple" href="https://bullz.jp/">Explore</v-btn>
            <v-spacer></v-spacer>
            <v-btn icon @click="show1 = !show1">
              <v-icon>{{ show1 ? 'keyboard_arrow_down' : 'keyboard_arrow_up' }}</v-icon>
            </v-btn>
          </v-card-actions>

          <v-slide-y-transition>
            <v-card-text v-show="show1">
              HTML, CSS(Sass), PHP等を活用し、WordPress対応のコーポレートサイトを作成しました。
            </v-card-text>
          </v-slide-y-transition>
        </v-card>
        <v-card class="mb-3">
          <img
            src="./assets/site-market.png"
            width="100%"
          >
          <v-card-title primary-title class="justify-center">
            <div>
              <div class="headline">SiteMarket</div>
              <span class="grey--text">サイトM&Aのサービスを開発しました。</span>
            </div>
          </v-card-title>

          <v-card-actions>
            <v-btn flat color="purple" href="https://www.site-market.jp/">Explore</v-btn>
            <v-spacer></v-spacer>
            <v-btn icon @click="show2 = !show2">
              <v-icon>{{ show2 ? 'keyboard_arrow_down' : 'keyboard_arrow_up' }}</v-icon>
            </v-btn>
          </v-card-actions>

          <v-slide-y-transition>
            <v-card-text v-show="show2">
              Rails, Bootstrap4, Heroku, Sendgrid等を活用し、独力でサイト売買サービスを開発しました。
            </v-card-text>
          </v-slide-y-transition>
        </v-card>
        <v-card class="mb-3">
          <img
            src="./assets/portfolio.png"
            width="100%"
          >
          <v-card-title primary-title class="justify-center">
            <div>
              <div class="headline">Toru Okada's Portfolio</div>
              <span class="grey--text">ポートフォリオサイトを作成しました。</span>
            </div>
          </v-card-title>

          <v-card-actions>
            <v-btn flat color="purple" href="https://toruokada.tokyo">Explore</v-btn>
            <v-spacer></v-spacer>
            <v-btn icon @click="show3 = !show3">
              <v-icon>{{ show3 ? 'keyboard_arrow_down' : 'keyboard_arrow_up' }}</v-icon>
            </v-btn>
          </v-card-actions>

          <v-slide-y-transition>
            <v-card-text v-show="show3">
              Vue.js + Vuetify + Firebaseにてポートフォリオサイトを作成しました。
            </v-card-text>
          </v-slide-y-transition>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
  </div>
</template>

<script>
export default {
  name: 'Portfolio',
  data: () => ({
    show1: false,
    show2: false,
    show3: false
  })
}
</script>

<style scoped>
.portfolio {
  margin-top: 30px;
}
</style>
