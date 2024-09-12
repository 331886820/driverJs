<template>
  <div id="app">
    <!--<img id="three" alt="Vue logo" src="./assets/logo.png">-->
    <DriverJs msg="Hi! YG...https://juejin.cn/user/501800125607752/posts"/>
  </div>
</template>

<script>
import DriverJs from './components/DriverJs.vue';

export default {
  name: 'App',
  components: {
    DriverJs
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
