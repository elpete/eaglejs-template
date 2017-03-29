<template lang="pug">
.eg-theme-agrume
  .eg-slideshow
    slide(enter='fadeIn' leave='bounceOutLeft')
      .center.frontpage
        h1 Eagle.js
        img(src='./logo.svg')
        h4 A Slideshow Framework for Vue.js
</template>

<script>
import eagle from 'eagle.js'

export default {
  mixins: [eagle.slideshow],
  infos: {
    title: 'My Slideshow',
    description: ''
  },
  data: function () {
    return {};
  }
}
</script>

<style lang='scss'>
@import 'node_modules/eagle.js/src/themes/agrume/agrume';

.frontpage {
  img {
    height: 7em;
  }
  img.control-schema {
    width: 8em;
    height: 3em;
  }
}
</style>
