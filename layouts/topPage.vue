<template>
  <div class="topPage">
    <HeaderNav />
    <nuxt />
  </div>
</template>
<script>
import HeaderNav from '~/components/header/HeaderNav.vue'
export default {
  layout: 'topPage',
  components: {
    HeaderNav
  }
}
</script>
<style scoped lang="scss">
.topPage {
  display: relative;
  margin: 0;
  padding: 0;
  // width: 100vw;
  // width: auto;
  // min-width: 100vw;
}
</style>
