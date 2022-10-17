<template>
  <nav>
    <router-link to="/"><span>00 </span>Home</router-link>
    <router-link to="/destionation"><span>01 </span>Destination</router-link>
    <router-link to="/crew"><span>02 </span>Crew</router-link>
    <router-link to="/technology"><span>03 </span>Technology</router-link>
  </nav>
  <router-view/>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
