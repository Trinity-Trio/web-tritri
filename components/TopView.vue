<template lang='pug'>
#topView
  img.logo(src='~/static/motionlogo.gif')
  img.guide(src='~/assets/loading.svg')
</template>
<script>
export default {
}
</script>

<style lang='sass' scoped>
#topView
  position: relative
  background-color: #03635B
  height: 100vh
  // min-height: 750px
  img.logo
    max-width: 80%
    max-height: 100%
    position: absolute
    top: 0
    bottom: 0
    left: 0
    right: 0
    margin: auto
  img.guide
    width: 80px
    height: 80px
    max-height: 15vh
    transform: rotate(180deg)
    position: absolute
    bottom: 5vh
    left: 0
    right: 0
    margin: auto
    animation: rotation 1s infinite ease
    animation-delay: 2s
    @keyframes rotation
      0%
        bottom: 5vh
      20%
        bottom: 4vh
      100%
        bottom: 5vh
</style>
