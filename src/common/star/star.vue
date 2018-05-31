<template>
  <div>
    <div class="stars">
      <img src="./starno.png" alt="" v-show="!show" @click="isShow">
      <img src="./staryes.png" v-show="show" alt="" @click="isShow">
      <img src="./starno.png" alt="" v-show="!show2" @click="isShow2">
      <img src="./staryes.png" v-show="show2" alt="" @click="isShow2">
      <img src="./starno.png" alt="" v-show="!show3" @click="isShow3">
      <img src="./staryes.png" v-show="show3" alt="" @click="isShow3">
      <img src="./starno.png" alt="" v-show="!show4" @click="isShow4">
      <img src="./staryes.png" v-show="show4" alt="" @click="isShow4">
      <img src="./starno.png" alt="" v-show="!show5" @click="isShow5">
      <img src="./staryes.png" v-show="show5" alt="" @click="isShow5">
      <span v-show="cshow5">非常好</span>
      <span v-show="cshow4">很好</span>
      <span v-show="cshow3">一般</span>
      <span v-show="cshow2">很差</span>
      <span v-show="cshow">非常差</span>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
  export default {
    data() {
      return {
        show:false,
        show2:false,
        show3:false,
        show4:false,
        show5:false,
      }

    },
    computed: {
      cshow5(){
        if(this.show && this.show2 && this.show3 && this.show4 && this.show5){
          return true
        }
      },
      cshow4(){
        if(this.show && this.show2 && this.show3 && this.show4 && !this.show5){
          return true
        }
      },
      cshow3(){
        if(this.show && this.show2 && this.show3 && !this.show4 && !this.show5){
          return true
        }
      },
      cshow2(){
        if(this.show && this.show2 && !this.show3 && !this.show4 && !this.show5){
          return true
        }
      },
      cshow(){
        if(this.show && !this.show2 && !this.show3 && !this.show4 && !this.show5){
          return true
        }
      },
    },
    methods:{
      isShow(){
        this.show = true
        this.show2 = false
        this.show3=false
        this.show4=false
        this.show5=false
      },
      isShow2(){
        this.show = true
        this.show2 = true
        this.show3=false
        this.show4=false
        this.show5=false
      },
      isShow3(){
        this.show = true
        this.show2 = true
        this.show3=true
        this.show4=false
        this.show5=false
      },
      isShow4(){
        this.show = true
        this.show2 = true
        this.show3=true
        this.show4=true
        this.show5=false
      },
      isShow5(){
        this.show = true
        this.show2 = true
        this.show3=true
        this.show4=true
        this.show5=true
      },
    }
  }
</script>

<style scoped lang="stylus">
.stars
  margin-left .12rem
  img
    width .28rem
  span 
    font-size .24rem
    margin-left .12rem
</style>
