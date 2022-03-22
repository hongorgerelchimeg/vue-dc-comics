<template>
  <div id="app">
    <main-header />
  </div>
</template>

<script>
import mainHeader from './components/mainHeader.vue'
// import mainContent from './components/main-content.vue'
// import mainFooter from './components/main-footer.vue'

export default {
  name: 'App',
  components: {
    mainHeader,
    // mainContent,
    // mainFooter
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
