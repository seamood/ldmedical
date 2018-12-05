<template>
  <div id='app'>
    <v-head></v-head>
    <router-view/>
    <v-foot class='foot'></v-foot>
  </div>
</template>

<script>
import foot from './components/foot.vue'
import head from './components/head'
export default {
  name: 'App',
  components: {
    'v-foot': foot,
    'v-head': head
  }
}
</script>

<style>
#app {
  height: 100%;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* margin-top: 60px; */
}
* {
  padding: 0;
  margin: 0;
}
.foot {
  position: fixed;
  bottom: 0;
  width: 100%;
}
html {
  height: 100%;
}
body {
  height: 100%;
}
</style>
