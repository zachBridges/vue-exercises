<template>
  <div id="app">
    <EmailUpdate/>
    <Thanks/>
  </div>
</template>

<script>
import { EmailUpdate, Thanks } from './views';
import User from './data/test-user';

export default {
  name: 'App',
  components: {
    EmailUpdate,
    Thanks,
  },
  data() {
    return {
      currentView: 'EmailUpdate',
      user: User.user,
    };
  },
  methods: {
    onUserUpdate(userData) {
      this.user = Object.assign({}, this.user, userData);
      this.currentView = 'EmailUpdate'
    },
  },
};
</script>


<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  padding: 1rem;
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

