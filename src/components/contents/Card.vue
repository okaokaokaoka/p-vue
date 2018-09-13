<template>
  <div class="card-wrapper">
    <v-container
          fluid
          grid-list-md
        >
    <v-card>
      <v-img src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
        height="200px"
      >
      </v-img>

      <v-card-title primary-title>
        <div>
          <div class="headline">岡田徹の友達はこんな感じ</div>
          <span class="grey--text">1,000人います</span>
        </div>
      </v-card-title>

      <v-card-actions>
        <v-btn flat>シェアする</v-btn>
        <v-btn flat color="purple">会う</v-btn>
        <v-spacer></v-spacer>
        <v-btn icon @click="show = !show">
          <v-icon>{{ show ? 'keyboard_arrow_down' : 'keyboard_arrow_up' }}</v-icon>
        </v-btn>
      </v-card-actions>

      <v-slide-y-transition>
        <v-card-text v-show="show">
          イガグリさんこんにちは
        </v-card-text>
      </v-slide-y-transition>
    </v-card>
  </v-container>
  </div>
</template>

<script>
export default {
  name: 'Card',
  data: () => ({
    show: false
  })
}
</script>

<style scoped>
.card-wrapper {
  margin-top: 30px;
}
</style>
