<template>
  <div class="toolbar" id="globalToolbar">
    <button type="button" id="addText">Text</button>
    <button type="button" class="colour" data-value="#05345C">Kent Blue</button>
    <button type="button" class="colour" data-value="#263566">Kent Light Blue</button>
    <button type="button" class="colour" data-value="#937227">Kent Gold</button>
  </div>
</template>

<script>

export default {
  name: 'global-tools',
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

</style>
