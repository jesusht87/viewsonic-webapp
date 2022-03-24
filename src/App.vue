<template>
  <div id="app">
    <nav>
      <img class="logo" src="@/assets/logo.png">
      <router-link to="/">🇪🇸 Español</router-link> |
      <router-link to="/english">🇬🇧 English</router-link> |
      <router-link to="/deutsch">🇩🇪 Deutsch</router-link>
    </nav>
    <router-view/>
  </div>
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
  padding: 25px;
  margin-right: 15%;
  text-align: right;
  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
.logo {
  display: block;
  max-width: 150px;
  margin-left: 15%;
}
</style>
