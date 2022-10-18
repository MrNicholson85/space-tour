<template>
  <div class="home">
    <h1>Home</h1>
  </div>
</template>
<script>
import planetInfo from '../assets/data/data.json'
import HomeBg from '@/assets/images/homepage-bg.png'

export default {
  data () {
    return {
      planetInfo,
      HomeBg
    }
  }
}
</script>
<style lang="scss">
@import '@/assets/scss/varibales.scss';

  .home {

  }
</style>
