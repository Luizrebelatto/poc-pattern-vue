<template>
  <img alt="Vue logo" src="./assets/logo.png">

  <UserAvatar/>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import UserAvatar from './components/userAvatar.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    UserAvatar
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
