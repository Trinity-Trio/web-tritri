<template lang='pug'>
#about
  h2 私達は<br>函館に<br>います
  section
    h3
      span T
      span r
      span i
      span n
      span i
      span t
      span y
      span T
      span r
      span i
      span o
    .verb
      p は３人である。
      p は情報機器を媒介として心の奥底に眠る思想や感情を表出する活動である。
      p はそれぞれの思考を融合した結果創出される結果である。
      p は共通の敵を持つ。
      p は音楽を扱う。
      p はテキストを扱う。
      p は空間を扱う。
      p は情報空間を扱う。
      p は函館の自分たちではどうにもならない憂鬱な雰囲気に対抗すべく、小さく抗う希望の灯火である。
      p は時間に制約されない。
      p は空間に制約されない。
</template>

<script>
export default {
}
</script>

<style lang='sass' scoped>
  #about
    // height: 75vh
    background-color: #03635B
    color: #fff
    text-align: center
    font-display: swap
    font-family: "Sawarabi Mincho", serif
    font-weight: bold
    padding: 7rem 0 7rem
    h2
      font-size: 5em
      margin: auto
      display: block
      padding: 1.45rem 1rem 1rem 1.4rem
      border: 2px solid #fff
      width: 3em
    section
      display: flex
      margin: 3rem 4rem 0
      font-size: 1vw
      justify-content: center
      @media screen and ( max-width : 1280px )
        font-size: .8rem
      h3
        font-family: 'Poppins', sans-serif
        writing-mode: vertical-rl
        font-size: 4.5em
        display: flex
        justify-content: space-between
        margin: .5rem 0 .5rem
      p
        font-size: 1.5em
        // margin-top: .25em
        margin-left: .1rem
        text-align: justify
        padding-left: 1em
        text-indent: -1em
        line-height: 1.7em
</style>
