<template>
  <div class="about">
    <div>
      <h1>
        岡田徹について紹介します
      </h1>
    </div>
    <Card/>
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
.about {
  margin-top: 50px;
}
</style>
