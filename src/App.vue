<template>
  <div id="app">
    <Login />
  </div>
</template>

<script>
import { mapActions } from 'vuex';
import Login from './components/Login.vue'

export default {
  name: 'app',
  components: {
    Login
  },
  methods: {
    ...mapActions([
      'fetchAccessToken'
    ]),
  },
  created() {
    this.fetchAccessToken();
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
