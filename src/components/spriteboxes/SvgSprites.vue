<template>
  <div class="sprite-box" id="kentgraphics" data-name="Kent Infographic graphics" data-type="inline-svg">
    <ul>
      <li data-addable="true"><svg width="55" height="41" viewBox="0 0 559 419"><use xlink:href="#degreescroll"/></svg> Degree scroll</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'svg-sprites',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
