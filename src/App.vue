<template>
  <div id="app">
    <h1 class="header m-4">Open Learing Server</h1>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/courses">Courses</router-link> |
      <router-link to="/sign-in">Sign In</router-link>
    </div>
    <router-view />
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
