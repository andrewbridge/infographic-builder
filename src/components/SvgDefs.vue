<template>
  <svg class="defs-only" xmlns="http://www.w3.org/2000/svg">
      <linearGradient id="coin" x2="50%" y2="40%" spreadMethod="reflect">
          <stop stop-color="gold" offset="30%"></stop>
          <stop stop-color="goldenrod" offset="70%"></stop>
          <stop stop-color="white" offset="82%"></stop>
          <stop stop-color="gold" offset="92%"></stop>
          <stop stop-color="darkgoldenrod" offset="100%"></stop>
      </linearGradient>
      <radialGradient id="pot" fx="30%" fy="35%">
          <stop stop-color="white" offset="0%"></stop>
          <stop stop-color="gold" offset="15%"></stop>
          <stop stop-color="goldenrod" offset="80%"></stop>
          <stop stop-color="darkgoldenrod" offset="100%"></stop>
      </radialGradient>
      <symbol id="potofgold">
          <g fill="url(#coin)" stroke="darkgoldenrod" stroke-width="0.5">
              <circle r="5" transform="translate(30,7)"></circle>
              <circle r="5" transform="translate(35,13)"></circle>
              <circle r="5" transform="translate(22,10)"></circle>
              <circle r="5" transform="translate(27,9)"></circle>
              <circle r="5" transform="translate(18,17)"></circle>
              <circle r="5" transform="translate(42,18)"></circle>
              <circle r="5" transform="translate(32,19)"></circle>
              <circle r="5" transform="translate(30,14)"></circle>
              <circle r="5" transform="translate(25,15)"></circle>
              <circle r="5" transform="translate(37,19)"></circle>
              <circle r="5" transform="translate(31,16)"></circle>
              <circle r="5" transform="translate(20,18)"></circle>
              <circle r="5" transform="translate(26,21)"></circle>
          </g>
          <path fill="url(#pot)" stroke="#751" stroke-width="0.5" d="M30,50 C45,50 55,45 55,35
                   Q 55,27 50,25 C55,22 53,15 45,20
                   S 23,25 15,20 S5,22 10,25
                   Q 5,27 5,35 C5,45 15,50 30,50Z"></path>
      </symbol>
      <symbol id="degreescroll">
        <path fill="#fff" class="cls-1" d="M83.76,282c-2.62-15.25-11.93-31.7-15.5-35.5-5.62-6-27.25-25.5-45.5,1.5-3.37,4.63-9.83,76.5,58,88.5,14.83,1.5,9.5-1.5,35-16.5s297.5-185.5,399.5-199.5c0,0,8,.5,7,11-4.5,20-198,64-407.5,226.5-67.25,35.25-151-99-98-139.5s207.5-68.5,357-186c74.13-58.26,99.5-20.5,99.5-20.5s46,46.5,43,75.5-68.5,28-158.5,80.5C330.33,184,97.34,310.7,88.26,316c-8.17,3.75-49-5.5-48.5-49s33.63,17,34.5,19.5S86.38,297.28,83.76,282Z"/><path fill="#896825" class="cls-2" d="M250.26,266.25s76-7.22,137,44.28c0,0,17.5-47.5,16.5-53.5l71-16S428,211.12,363.51,206.12V206C329.13,222.46,291,242,250.29,266.13,250.1,266.43,250.26,266.25,250.26,266.25Z"/><path class="cls-3" d="M250.07,266.48l-.27.43Z"/><path fill="#937227" class="cls-3" d="M250.24,266.19c40.7-24.14,78.89-43.66,113.27-60.07h0l2.25-51.58s-5.91-54.75-72.41-66.75c0,0-113.53,58.22-120.76,60.58,0,0,65.67-1.83,80.17,45.67,13.43,44-.38,68.71-2.52,72.16Z"/>
      </symbol>
  </svg>
</template>

<script>

export default {
  name: 'svg-defs',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
svg.defs-only {
  display: block;
  position: absolute;
  height: 0;
  width: 0;
  margin: 0;
  padding: 0;
  border: none;
  overflow: hidden;
}
</style>
