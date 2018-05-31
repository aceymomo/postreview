<template>
  <div>
    <post-header></post-header>
    <post-mid></post-mid>
    <post-bottom></post-bottom>
  </div>
</template>

<script type="text/ecmascript-6">
import PostHeader from '@/components/pages/header'
import PostMid from '@/components/pages/mid'
import PostBottom from '@/components/pages/bottom'
  export default {
    data() {
      return {

      }

    },
    components: {
      PostHeader,
      PostMid,
      PostBottom
    }
  }
</script>

<style scoped lang="stylus">

 
</style>
