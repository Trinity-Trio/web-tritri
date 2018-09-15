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
  display: flex
  flex-direction: column
  align-items: center
  justify-content: center
  height: 100vh
  background-color: #03635B
  img.logo
    max-width: 80%
  img.guide
    width: 80px
    height: 80px
    animation: rotation 1.55s infinite ease
    animation-delay: 2s
    @keyframes rotation
      0%
        transform: rotate(-60deg)
      50%
        transform: rotate(180deg)
      100%
        transform: rotate(180deg)
</style>
