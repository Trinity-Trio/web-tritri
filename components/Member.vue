<template lang='pug'>
#member
  #CHARLII_k.item
    img(src='~/assets/memberCHARLII_k.svg')
    p CHARLII_k
  #ryu-g.item
    img(src='~/assets/memberryu-g.svg')
    p ryu-g
  #by_sK.item
    img(src='~/assets/memberby_sK.svg')
    p by_sK
</template>

<script>
export default {
}
</script>

<style lang='sass' scoped>
#member
  height: 100vh
  display: grid
  grid-template-columns: .92fr 1fr .94fr
  @media screen and ( max-width : 768px )
    grid-template-columns: none
    grid-template-rows: .92fr 1fr .90fr

#CHARLII_k
  background-color: #FFCC00
  color: #FFCC00
#ryu-g
  background-color: #E95513
  color: #E95513
#by_sK
  background-color: lighten(#4e1a68, 25%)
  color: lighten(#4e1a68, 25%)

.item
  position: relative
  // text-align: center
  overflow: hidden
  img
    position: absolute
    bottom: -1rem
    height: 100vh
    left: 50%
    right: 50%
    transform: translateX(-50%)
    z-index: 1
    // transition: .2s
    @media screen and ( max-width : 768px )
      transition: none
      top: -70vh
      bottom: auto
      height: 220vh
      left: 25%
  p
    position: absolute
    left: 2rem
    bottom: 2rem
    z-index: 2
    font-size: 1.5rem
    font-weight: bold
    background-color: #000
    padding: 0 .2em .2em
    height: 1em
    @media screen and ( max-width : 768px )
      left: 1rem
      top: 1rem
      font-size: 1.2rem
  // &:hover
  //   img
  //     bottom: 0rem
</style>
