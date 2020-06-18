<template>
    <div>
      <div class="profile">
        <Header-Top title="我的"></Header-Top>
        <div class="profile-number">

        <router-link to='login' class="profile-link">
                  <div class="profile-image">
              <i class="iconfont icon-touxiang"></i>
            </div>
            <div class="user-info">
              <p class="user-info-top">登录/注册</p>
              <p>
                <span class="user-icon">
                  <i class="iconfont icon-shouji1"></i>
                </span>
                <span class="icon-mobile-number">暂无绑定手机号</span>
              </p>
            </div>
            <span class="arrow">
              <i class="iconfont icon-icon-jiantou1"></i>
            </span>
        </router-link>
          
        </div>
        <div class="profile-info-data border-1px">
          <ul class="info-data-list">
            <a href="javascript:" class="info-data-link">
              <span class="info-data-top"><span>0.00</span>元</span>
              <span class="info-data-bottom">我的余额</span>
            </a>
            <a href="javascript:" class="info-data-link">
              <span class="info-data-top"><span>0</span>个</span>
              <span class="info-data-bottom">我的优惠</span>
            </a>
            <a href="javascript:" class="info-data-link">
              <span class="info-data-top"><span>0</span>分</span>
              <span class="info-data-bottom">我的积分</span>
            </a>
          </ul>
        </div>
        <div class="profile-my-order border-1px">
          <!-- 我的订单 -->
          <a href='javascript:' class="my-order">
            <span>
              <i class="iconfont icon-icon-order-s"></i>
            </span>
            <div class="my-order-div">
              <span>我的订单</span>
              <span class="my-order-icon">
                <i class="iconfont icon-icon-jiantou1"></i>
              </span>
            </div>
          </a>
          <!-- 积分商城 -->
          <a href='javascript:' class="my-order">
            <span>
              <i class="iconfont icon-iconjifen"></i>
            </span>
            <div class="my-order-div">
              <span>积分商城</span>
              <span class="my-order-icon">
                <i class="iconfont icon-icon-jiantou1"></i>
              </span>
            </div>
          </a>
          <!-- 硅谷外卖会员卡 -->
          <a href="javascript:" class="my-order">
            <span>
              <i class="iconfont icon-iconvip"></i>
            </span>
            <div class="my-order-div">
              <span>硅谷外卖会员卡</span>
              <span class="my-order-icon">
                <i class="iconfont icon-icon-jiantou1"></i>
              </span>
            </div>
          </a>
        </div>
        <div class="profile-my-order border-1px">
          <!-- 服务中心 -->
          <a href="javascript:" class="my-order">
            <span>
              <i class="iconfont icon-icon-fuwu"></i>
            </span>
            <div class="my-order-div">
              <span>服务中心</span>
              <span class="my-order-icon">
                <i class="iconfont icon-icon-jiantou1"></i>
              </span>
            </div>
          </a>
        </div>
      </div>
    </div>
</template>

<script>
import HeaderTop from '../../components/HeaderTop/HeaderTop.vue'
export default {
      components : {
            HeaderTop
      }
}
</script>

<style lang='stylus' rel='stylesheet/stylus'>

@import '../../common/stylus/mixins.styl'

.profile
  width 100%
  overflow hidden
  .header
    background-color #02a774
    position fixed
    z-index 100
    left 0
    top 0
    width 100%
    height 45px
    .header-title
      position absolute
      top 50%
      left 50%
      transform translate(-50%,-50%)
      width 48%
      color #ffffff
      font-size 22px
      text-align center
      .header-title-text
        font-size 20px
        color #ffffff
        display block
  .profile-number
    margin-top 45.5px
    .profile-link
      clearFix()
      position relative
      display block
      background #02a774
      padding 20px 10px
      color #fff
      .profile-image
        float left
        width 60px
        height 60px
        border-radius 50%
        overflow hidden
        vertical-align top
        .icon-touxiang
          background #e4e4e4
          font-size 62px
      .user-info
        float left
        margin-top 8px
        margin-left 15px
        p
          font-weight: 700
          font-size 18px
          color #fff
          &.user-info-top
            padding-bottom 8px
          .user-icon
            display inline-block
            margin-left -15px
            margin-right 5px
            width 20px
            height 20px
            .icon-shouji1
              font-size 30px
              vertical-align text-top
          .icon-mobile-number
            font-size 14px
            color #fff
      .arrow
        width 12px
        height 12px
        position absolute
        right 15px
        top 40%
        .icon-icon-jiantou1
          color #ffffff
          font-size 5px
  .profile-info-data
    bottom-border-1px(#e4e4e4)
    width 100%
    background #fff
    overflow hidden
    .info-data-list
      clearFix()
      .info-data-link
        float left
        width 33%
        text-align center
        border-right 1px solid #f1f1f1
        text-decoration none
        .info-data-top
          display block
          width 100%
          font-size 14px
          color #333
          padding 15px 5px 10px
          span
            display inline-block
            font-size 30px
            color #f90
            font-weight 700
            line-height 30px
        .info-data-bottom
          display inline-block
          font-size 14px
          color #666
          font-weight 400
          padding-bottom 10px
      .info-data-link:nth-of-type(2)
        .info-data-top
          span
            color #ff5f3e
      .info-data-link:nth-of-type(3)
        border 0
        .info-data-top
          span
            color #6ac20b
  .profile-my-order
    top-border-1px(#e4e4e4)
    margin-top 10px
    background #fff
    .my-order
      display flex
      align-items center
      padding-left 15px
      text-decoration none
      >span 
        display flex
        align-items center
        width 20px
        height 20px
        >.iconfont
          margin-left -10px
          font-size 30px
        .icon-icon-order-s
          color #02a774
        .icon-iconjifen
          color #ff5f3e
        .icon-iconvip
          color #f90
        .icon-icon-fuwu
          color #02a774
      .my-order-div
        width 100%
        border-bottom 1px solid #f1f1f1
        padding 18px 10px 18px 0
        font-size 16px
        color #333
        display flex
        justify-content space-between
        span 
          display block
        .my-order-icon
          width 10px
          height 10px
          .icon-icon-jiantou1
            color #bbb
            font-size 10px











</style>