<template>
  <div class="portfolio">
  <v-layout row>
    <v-flex xs12 sm6 offset-sm3>
      <v-card>
        <v-img
          src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
          height="200px"
        >
        </v-img>
        <v-card-title primary-title>
          <div>
            <div class="headline">Bullz Hompage</div>
            <span class="grey--text">株式会社ブルズのホームページを改修しました。</span>
          </div>
        </v-card-title>

        <v-card-actions>
          <v-btn flat color="purple">Explore</v-btn>
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
      <v-card>
        <v-img
          src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
          height="200px"
        >
        </v-img>

        <v-card-title primary-title>
          <div>
            <div class="headline">SiteMarket</div>
            <span class="grey--text">サイトM&Aのサービスを開発しました。</span>
          </div>
        </v-card-title>

        <v-card-actions>
          <v-btn flat color="purple">Explore</v-btn>
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
    </v-flex>
  </v-layout>
  </div>
</template>

<script>
export default {
  name: 'Portfolio',
  data: () => ({
    show1: false,
    show2: false
  })
}
</script>

<style scoped>
.portfolio {
  margin-top: 30px;
  margin-right: 10px;
  margin-left: 10px;
}
</style>
