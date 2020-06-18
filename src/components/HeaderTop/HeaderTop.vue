<template>
               <div class="header">
                     <slot name="left"></slot>
                     <span class="header-title">
                             <span class="header-title-text ellipsis">{{title}}</span>
                     </span>
                     <slot name="right"></slot>
             </div>
</template>

<script>
export default {

   props : {
     title: String
   }

}
</script>

<style lang="stylus" rel="stylesheet/stylus">
.header
  background-color #02a774
  position fixed
  z-index 100
  left 0
  top 0
  width 100%
  height 45px
  .header-search
    position absolute
    left 15px
    top 50%
    transform  translateY(-50%)
    width 10%
    height 50%
    .iconfont
      font-size 22px
      color #fff
  .header-title
    position absolute
    top 50%
    left 50%
    transform translate(-50%,-50%)
    width 48%
    color #fff
    font-size 22px
    text-align center    
    .header-title-text
      font-size 20px
      color #fff
      display block
  .header-login
    font-size 14px
    color #ffffff
    position absolute
    right 15px
    top 50%
    transform translateY(-50%)
    width 17%
    .header-login-text
      color #fff
</style>