<template>
  <div id="app">
    <mainHeader />
    <mainContent />
    <mainFooter />
  </div>
</template>

<script>
import mainHeader from './components/mainHeader.vue'
import mainContent from './components/mainContent.vue'
import mainFooter from './components/mainFooter.vue'

export default {
  name: 'App',
  components: {
    mainHeader,
    mainContent,
    mainFooter
  }
}
</script>

<style lang="scss">
@import "./assets/styles/main";

</style>
