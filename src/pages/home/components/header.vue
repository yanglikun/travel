<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>输入框
    </div>
    <div class="header-right">城市<span class="iconfont cityarrow">&#xe64a;</span></div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>
<style lang="stylus" scoped>
  @import "~style/variables.styl"
  .header
    line-height 0.86rem
    background-color: $bgcolor
    display flex

    .header-left
      width: .64rem
      float: left
      text-align center

    .header-input
      flex 1
      padding-left 0.2rem
      height: 0.64rem
      line-height: 0.64rem
      margin-top: .12rem
      margin-left .2rem
      background-color: #ffffff
      border-radius: .1rem
      color: #ccc

    .header-right
      width: 1.24rem
      float: right
      text-align center

      .cityarrow
        font-size 0.3rem
</style>
