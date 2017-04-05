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
    position:fixed;
    top: 0;
    left: 0;
    right: 0;
    width: 100vw;
    height: $headerHeight;
    background: $headerColour;
    color: white;
  }

  h1 {
    font-size: 18px;
    padding: 0;
    margin: 0;
  }
</style>
