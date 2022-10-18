<template>
  <Nav/>
  <router-view/>
</template>
<script>
import Nav from '@/components/Nav.vue'

export default {
  name: 'App',
  components: { Nav }
}
</script>
<style lang="scss">
@import '@/assets/scss/typography.scss';

body {
  background-color: $nior;
  padding: 0;
  margin: 0;
}

#app {
  font-family: $barlowReg;
  color: $white;
}
</style>
