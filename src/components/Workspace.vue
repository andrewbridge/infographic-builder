<template>
  <div class="workspace">
    <div class="build-area-container">
      <div class="svg-build-area">
        <svg id="build-area"></svg>
        <canvas id="controls" class="underlay"></canvas>
      </div>
      <div id="build-area-resizer" class="resizer"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'workspace',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.workspace {
  width: 100%;
  height: calc(100vh - 100px);
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #282828;
}
</style>
