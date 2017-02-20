<template>
  <div class="control-panel-container">
    <control-panel id="object-attributes" snap="top">
      <global-tools></global-tools>
      <text-tools></text-tools>
      <icon-tools></icon-tools>
    </control-panel>
    <control-panel id="object-selector" snap="left">
      <svg-sprites></svg-sprites>
      <fontawesome-sprites></fontawesome-sprites>
    </control-panel>
  </div>
</template>

<script>
import ControlPanel from 'components/ControlPanel'
import GlobalTools from 'components/toolbars/GlobalTools'
import TextTools from 'components/toolbars/TextTools'
import IconTools from 'components/toolbars/IconTools'
import SvgSprites from 'components/spriteboxes/SvgSprites'
import FontawesomeSprites from 'components/spriteboxes/FontawesomeSprites'

export default {
  name: 'control-panels',
  components: {
    ControlPanel,
    GlobalTools,
    TextTools,
    IconTools,
    SvgSprites,
    FontawesomeSprites
  },
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
