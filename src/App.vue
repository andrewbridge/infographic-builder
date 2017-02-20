<template>
  <div id="app">
    <svg-defs></svg-defs>
    <app-header></app-header>
    <control-panels></control-panels>
    <workspace></workspace>
  </div>
</template>

<script>
import SvgDefs from 'components/SvgDefs'
import AppHeader from 'components/AppHeader'
import ControlPanels from 'components/ControlPanels'
import Workspace from 'components/Workspace'

export default {
  name: 'app',
  components: {
    SvgDefs,
    AppHeader,
    ControlPanels,
    Workspace
  }
}
</script>

<style lang="scss">
@import '~mdl/material.min.css';

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
