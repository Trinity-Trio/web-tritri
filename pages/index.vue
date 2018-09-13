<template lang='pug'>
section.container
  TopView
  Member
  About
  Works
</template>

<script>
import TopView from '~/components/TopView.vue'
import Member from '~/components/Member.vue'
import About from '~/components/About.vue'
import Works from '~/components/Works.vue'

export default {
  components: {
    TopView,
    Member,
    About,
    Works
  }
}
</script>

<style lang='sass'>
body
  background-color: #03635B
</style>
