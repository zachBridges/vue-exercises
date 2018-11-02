<template>
  <div id="app">
    <img src="https://media0.giphy.com/media/fedryX7dMGMe6lgqDm/giphy.gif?cid=3640f6095bd895c8794e7a466bb07658" alt="Hello World"/>
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
