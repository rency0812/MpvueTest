<template>
  <div class="homepage">
    <music></music>
    <div class="content">
      <div class="avatar">
        <img :src="imgSrc" class="avatar-item">
      </div>
      <h1 class="description">相信自己、比谁都棒。</h1>
      <ul class="tab">
        <li class="tab-item">
          <a class="tab-link" href="../blog/blog">新浪博客</a>
        </li>
        <li class="tab-item">
          <a class="tab-link" href="../works/works">工作经历</a>
        </li>
        <li class="tab-item">
          <a class="tab-link" href="../error/error?id=2">GitHub</a>
        </li>
        <li class="tab-item">
          <a class="tab-link" href="../me/me">关于我</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
  import Music from '@/components/music'

  export default {
    components: {
      Music
    },
    data () {
      return {
        imgSrc: '/static/img/5.png'
      }
    }
  }
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
  .homepage
    position: relative
    height: 100vh
    overflow: hidden
    background: #fff
    z-index: 3
    .content
      position :absolute
      top: 0
      left: 0
      width: 100%
      height: 100%
      display: flex
      flex-direction: column
      align-items: center
      justify-content: center
      z-index: 3
      text-align: center
      .avatar
        margin-bottom: 20px
        img
          width: 120px
          height: 120px
          overflow: hidden
          border-radius: 50%
          background: #FFF
          box-shadow: rgba(255, 255, 255, 0.1) 0 0 0 5px, rgba(0, 0, 0, 0.1) 0 0 5px 4px
          transition: transform .4s ease-out
        img:hover
          transform: rotate(360deg)
      .description
        margin-bottom: 20px
        font-weight: bold
        color: #6289ad
        font-size: 24px
      .tab
        .tab-item
          height: 40px
          line-height: 40px
          text-align: center
          list-style: none
          .tab-link
            padding: 10px
            color:#666
            font-size: 14px
            font-weight: 600
          a:hover
            color: #6289ad
            font-weight: 700
</style>
