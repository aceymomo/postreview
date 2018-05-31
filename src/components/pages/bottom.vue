<template>
  <div>
    <div class="title">
      <div class="left">
        <span>ORD:3469489746489</span>
      </div>
      <div class="right">
        <span>Seller:</span>
        <strong>FREEZBUY</strong>
      </div>
    </div>
    <div class="bt-content">
      <div class="content-img">
        <img src="./dress.png" alt="">
      </div>
      <div class="content-font">
        <span>Sheath/Column Elastic Satin Sweep... 
Sheath/Column Elastic Satin Sweep...</span>
      </div>
    </div>
    <div class="bt-star">
      <span>Satisfaction:</span>
      <star></star>
    </div>
    <div class="bt-input">
      <textarea placeholder="Place leave a detailed review, your reivew is very important for orther buyer."></textarea>
    </div>
    <div class="bt-upload">
      <upload></upload>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
import Star from '@/common/star/star'
import Upload from '@/common/upload/upload'
  export default {
    data() {
      return {
        
      }

    },
    components: {
      Star,
      Upload
    },
    methods:{
      
    }
  }
</script>

<style scoped lang="stylus">
.title
  padding .24rem .2rem
  border-bottom 1px solid #c4c4c5
  display flex
  justify-content space-between
  .left
    span
      font-size .24rem
  .right
    font-size .24rem
    strong
      color #d42727
.bt-content
  padding .24rem .2rem
  display flex
  .content-img
    img
      width 1.2rem
  .content-font
    padding .3rem 0
    margin-left .16rem
    width 60%
    max-height .56rem
    overflow hidden
    span
      line-height .48rem
      font-size .24rem
.bt-star
  padding .24rem .2rem
  display flex
  border-bottom 1px solid #efefef
  span
    font-size .28rem
.bt-input
  padding .24rem .2rem
  textarea
    padding .08rem .12rem
    width 100%
    font-size .28rem
.bt-upload
  padding .24rem .2rem
</style>
