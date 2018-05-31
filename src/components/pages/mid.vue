<template>
  <div>
    <div class="title">
      <img src="./colo.png" alt="">
      <span>Overall Rating</span>
    </div>
    <div class="pl">
      <div class="pl-content">
        <img src="./good.png" alt="">
        <span>Positive</span>
      </div>
      <div class="pl-content">
        <img src="./normal.png" alt="">
        <span>Neutral</span>
      </div>
      <div class="pl-content">
        <img src="./loss.png" alt="">
        <span>Negative</span>
      </div>
    </div>
    <div class="star">
      <div class="star-box">
        <span>Communication :</span>
        <div class="stars">
          <star></star>
        </div>
      </div>
      <div class="star-box">
        <span>Items as described :</span>
        <div class="stars">
          <star></star>
        </div>
      </div>
      <div class="star-box">
        <span>Shipping & Delivery :</span>
        <div class="stars">
          <star></star>
        </div>
      </div>
    </div>
    <div class="class-bottom"></div>
  </div>
</template>

<script type="text/ecmascript-6">
import Star from '@/common/star/star'
  export default {
    data() {
      return {

      }

    },
    components: {
      Star
    }
  }
</script>

<style scoped lang="stylus">
.title
  padding .24rem .2rem
  border-bottom 1px solid #c4c4c5
  img
    width .28rem
  span
    font-size .28rem
    margin-left .12rem
.pl
  padding .24rem .2rem
  display flex
  .pl-content
    flex 1
    img
      width .3rem
    span
      font-size .3rem
      margin-left .12rem
.star
  padding .24rem .2rem
  margin-top .2rem
  .star-box
    position relative
    margin-bottom .2rem
    span
      font-size .28rem
    .stars
      position absolute
      top 0
      left 3rem
      img
        width .28rem
.class-bottom
  width 100%
  height .14rem
  background #efefef
</style>
