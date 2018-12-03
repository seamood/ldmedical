<template>
  <div id="app">
    <router-view/>
    <v-foot></v-foot>
  </div>
</template>

<script>
import foot from './components/foot.vue'
export default {
  name: 'App',
  components: {
    'v-foot': foot
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* margin-top: 60px; */
}
*{
  padding: 0;
  margin: 0;
}
</style>
