<template>
  <div id="app">
    <a href="https://github.com/vuejs-templates/webpack-simple"
       title="Webpack simple template"
       target="_blank"
       rel="tipsy">Hover over me</a>
  </div>
</template>

<script>
import $ from 'jquery'
import tipsy from 'jtipsy'

export default {
  name: 'app',
  mounted () {
    $('a[rel=tipsy]').tipsy({fade: true, gravity: 'n'})
  }
}
</script>

<style lang="less">
  @import "../node_modules/jtipsy/src/jquery.tipsy.css";
</style>
