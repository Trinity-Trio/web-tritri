<template lang='pug'>
#member
  #CHARLII_k.item(@click='charlii')
    img(src='~/assets/memberCHARLII_k.svg')
    p CHARLII_k
  #ryu-g.item(@click='ryu')
    img(src='~/assets/memberryu-g.svg')
    p ryu-g
  #by_sK.item(@click='sk')
    img(src='~/assets/memberby_sK.svg')
    p by_sK
</template>

<script>
export default {
  data: () => {
    return {
    }
  },
  methods: {
    charlii: () => {
      console.log('cha')
    },
    ryu: () => {
      console.log('ryu')
    },
    sk: () => {
      console.log('sk')
    }
  }
}
</script>

<style lang='sass' scoped>
// pc
$cha-w: .92
$ryu-w: 1
$sk-w: .94

// sp
$cha-h: .92
$ryu-h: 1
$sk-h: 90

#member
  height: 100vh
  display: flex
  flex-direction: row
  @media screen and ( max-width : 768px )
    flex-direction: column

#CHARLII_k
  background-color: #FFCC00
  color: #FFCC00
  flex-grow: $cha-w
  @media screen and ( max-width : 768px )
    flex-grow: $cha-h
#ryu-g
  background-color: #E95513
  color: #E95513
  flex-grow: $ryu-w
  @media screen and ( max-width : 768px )
    flex-grow: $ryu-h
#by_sK
  background-color: lighten(#4e1a68, 25%)
  color: lighten(#4e1a68, 25%)
  flex-grow: $sk-w
  @media screen and ( max-width : 768px )
    flex-grow: $sk-h

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
