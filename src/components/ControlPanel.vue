<template>
  <div class="control-panel" :data-snap="snap">
    <slot></slot>
  </div>
</template>

<script>

export default {
  name: 'control-panel',
  props: ['snap'],
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

 .control-panel {
    position: fixed;
    background: $panelColour;
    z-index: 10;
  }

  [data-snap="left"] {
        left: 0;
        top: $headerHeight;
        bottom: 0;
        height: calc(100vh - $headerHeight);
        width: 162px;
        overflow: scroll;
        padding: 0 3px;
        border-right: 1px solid #383838;
      }

      [data-snap="top"] {
        left: 169px;
        right: 0;
        top: $headerHeight;
        height: 100px;
        width: calc(100vw - 165px);
        padding: 3px;
        border-bottom: 1px solid #383838;
      }
</style>
