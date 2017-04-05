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
<style scoped lang="scss">
  @import "src/variables.scss";

.workspace {
  width: 100%;
  height: calc(100vh - 100px);
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: $bgColour;
}

.build-area-container {
  position: relative;
  display: inline-block;
  background: url("~assets/images/canvas-background.png");
}

.svg-build-area {
  border: 1px solid #383838;
  display: inline-block;
  position: relative;
  z-index: 0;
  overflow: hidden;
}
.svg-build-area * {
  user-select: none;
}
.svg-build-area svg *:hover, .resizer {
  cursor: move;
}
.resizer::after {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f0b2";
  color: #383838;
  position: absolute;
  bottom: -20px;
  right: -20px;
}
.controls {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1;
}
</style>
