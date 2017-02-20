<template>
  <div class="toolbar" id="iconToolbar">
    <button type="button" class="colour" data-value="#05345C">Kent Blue</button>
    <button type="button" class="colour" data-value="#263566">Kent Light Blue</button>
    <button type="button" class="colour" data-value="#937227">Kent Gold</button>
    <button type="button" class="colour" data-value="#FFFFFF">White</button>
  </div>
</template>

<script>

export default {
  name: 'icon-tools',
  components: {},
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
