<template>
  <main>
      <div class="container">

          <h1>Content Goes Here!</h1>
      </div>
  </main>
</template>

<script>
export default {
    name: 'mainContent'
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/main"; 
main {
    background-color: $mainBgContent;
    color: white;
    .container {
        padding: 3rem 0;
    }
}
</style>