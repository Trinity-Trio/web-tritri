<template lang='pug'>
#works
  .box
    iframe.song(scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/493909566&color=%2300aabb&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true")
    img.loading( src="~/static/wait.svg" alt="loading" width=200)
  .box
    iframe.song(scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/493909692&color=%2300aabb&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true")
    img.loading( src="~/static/wait.svg" alt="loading" width=200)
  .box
    iframe.song(scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/493909863&color=%2300aabb&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true")
    img.loading( src="~/static/wait.svg" alt="loading" width=200)
  .box
    iframe.song(scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/493910124&color=%2300aabb&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true")
    img.loading( src="~/static/wait.svg" alt="loading" width=200)
  .box
    iframe.song(scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/493910787&color=%2300aabb&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true")
    img.loading( src="~/static/wait.svg" alt="loading" width=200)
  .box
    iframe.song(scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/493911225&color=%2300aabb&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true")
    img.loading( src="~/static/wait.svg" alt="loading" width=200)
  .box
    iframe.song(scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/494605326&color=%2300aabb&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true")
    img.loading( src="~/static/wait.svg" alt="loading" width=200)
</template>

<script>
export default {
}
</script>

<style lang='sass' scoped>
  #works
    display: flex
    flex-wrap: wrap
    .box:nth-child(3n+1)
      background-color: #FFCC00
    .box:nth-child(3n+2)
      background-color: #e95513
    .box:nth-child(3n)
      background-color: #9A35CD
    .song
      z-index: 1
      width: 100%
      height: 100%
    .box
      display: flex
      justify-content: center
      align-items: center
      width: calc(100vw / 3)
      height: calc(100vw / 3)
      @media screen and (max-width:768px)
        width: 50vw
        height: 50vw
      @media screen and (max-width:411px)
        width: 100%
        height: 100vw
      .loading
        position: absolute
        z-index: 0
        width: 150px
        height: 150px
        animation: rotation 1s infinite ease-in-out
        @keyframes rotation
          0%
            transform: rotate(0deg)
          100%
            transform: rotate(358deg)
</style>
