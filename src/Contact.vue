<template>
  <div class="contact">
    <div class="mt-3">
    <p class="display-1">Contact.</p>
    </div>
    <div class="mt-3 contact-wrapper">
      <p>mail: toruhandbell0424@gmail.com</p>
      <p>twitter: https://twitter.com/okaokatoru</p>
      <p>facebook: https://www.facebook.com/okyaokya.yanen</p>
      <p class="cta-txt">お気軽にお問い合わせください</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Contact'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.contact-wrapper {
  font-size: 18px;
}
.cta-txt {
  font-size: 20px;
  font-weight: bold;
}
@media (max-width: 480px) {
  .contact-wrapper {
    font-size: 16px;
  }
  .cta-txt {
    font-size: 18px;
    font-weight: bold;
  }
}
</style>
