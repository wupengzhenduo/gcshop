<template>
     <div class="search">

          <Header-Top title="搜索"></Header-Top>
          

          <form action="#" class="search-form">
                    <input type="search" name="search" placeholder="请输入商家名称或美食名称" class="search-input">
                    <input type="submit" name="submit" class="search-submit">
          </form>
     </div>
</template>

<script>
import HeaderTop from "../../components/HeaderTop/HeaderTop.vue"

export default {
    components : {
      HeaderTop
    }

}
</script>

<style lang='stylus' rel='stylesheet/stylus'>

     @import  "../../common/stylus/mixins.styl";

     .search //搜索
          width 100%
          .search-form
               clearFix()
               margin-top 45px
               background-color #ffffff
               padding 12px 8px
               input
                    height 35px
                    padding 0px 4px
                    border-radius 2px
                    font-weight bold
                    outline none
               .search-input
                    float left
                    width 79%
                    border 4px solid #f2f2f2
                    font-size 14px
                    color #333
                    background-color #f2f2f2                   
               .search-submit
                    float right
                    width 18%
                    border 4px solid #02a774
                    font-size 16px
                    color #ffffff
                    background-color #02a774
</style>