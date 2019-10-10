<template>
  <div id="app">
    <div id="nav">
    <md-tabs class="md-primary" md-alignment="centered">
      <md-tab id="tab-home" md-label="Home">
        <router-link to="/"></router-link> |
      </md-tab>
      <md-tab id="tab-about" md-label="About">
        <router-link to="/about"></router-link>
      </md-tab>
    </md-tabs>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
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
