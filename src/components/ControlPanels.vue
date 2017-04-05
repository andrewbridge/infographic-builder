<template>
  <div class="control-panel-container">
    <control-panel class="show" id="object-attributes" snap="top">
      <global-tools v-if="attributes === 'global'"></global-tools>
      <text-tools v-else-if="attributes === 'text'"></text-tools>
      <icon-tools v-else-if="attributes === 'icon'"></icon-tools>
    </control-panel>
    <control-panel class="show" id="object-selector" snap="left">
      <svg-sprites v-if="selector === 'svg'"></svg-sprites>
      <fontawesome-sprites v-else-if="selector === 'fontawesome'"></fontawesome-sprites>
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
      selector: 'svg',
      attributes: 'global'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.control-panel, .toolbar, .sprite-box {
  display: none;
  &.show {
    display: block;
  }
}
</style>
