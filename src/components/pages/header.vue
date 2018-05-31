<template>
  <div>
    <div class="header">
      <div class="left">
        <img src="./left.png" alt="">
      </div>
      <div class="mid">Post Review</div>
      <div class="right">Confirm</div>
    </div>
    <div class="header-bot">
      <div class="bot-icon">
        <img src="./taobao.png" alt="">
      </div>
      <div class="bot-num">
        <div class="num-1">
          <img src="./num1.png" alt="">
          <span>215</span>
        </div>
        <div class="num-1">
          <img src="./num2.png" alt="">
          <span>98.2%</span>
        </div>
      </div>
      <div class="bot-font">
        <span>Transactions</span>
        <span>Positive Feedback</span>
      </div>
    </div>
    <div class="class-bottom"></div>
  </div>
</template>

<script type="text/ecmascript-6">
  export default {
    data() {
      return {

      }

    },
    components: {

    }
  }
</script>

<style scoped lang="stylus">
.header
  padding .24rem 0
  display flex
  justify-content space-between
  align-items center
  position relative
  border-bottom 1px solid #c4c4c5
  .left
    width .14rem
    margin-left .2rem
    img
      width 100%
  .mid
    width 100%
    text-align center
    position absolute
    font-size .3rem
  .right
    font-size .24rem
    color #d42727
    margin-right .2rem
.header-bot
  padding .24rem .2rem
  display flex
  .bot-icon
    width 1.2rem
    height 1.2rem
    img
      width 100%
      height 100%
  .bot-num
    padding .14rem 0
    margin-left .32rem
    .num-1
      margin-bottom .26rem
      img
        width .24rem
      span
        font-size .24rem
        margin-left .2rem
        color #3366ff
  .bot-font
    margin-left .18rem
    padding .14rem 0
    span
      display block
      font-size .24rem
      margin-bottom .32rem
.class-bottom
  width 100%
  height .14rem
  background #efefef
</style>
