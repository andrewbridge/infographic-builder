<template>
  <header>
    <h1>Infographic Builder</h1>
  </header>
</template>

<script>
export default {
  name: 'app-header',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import "src/variables.scss";

  header {
    background: black;
    color: white;
  }
</style>
