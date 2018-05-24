<template>
  <div class="me" :class="{'detail': show}">
    <navigation :me="1" @show="showgun"></navigation>
    <div class="page">
      <div class="blog-detail">
        <div class="blog-detail-contaner">
          <div class="header">
            <div class="header-cover no-cover">
              <div class="header-body">
                <div class="avatar">
                  <img src="/static/img/5.png" class="avatar-item">
                </div>
                <div class="tit">rency</div>
              </div>
            </div>
          </div>
          <div class="article-section">
            <div class="article markdown-body">
              <ul>
                <li>熟练使用移动端h5页面的视觉设计和布局，兼容各种主流移动设备</li>
                <li>利用HTML/CSS/JavaScript/CSS3/HTML5/jQuery等各种Web技术进行产品的界面开发。使用原生js写页面的动态交互，解决主流浏览器的兼容问题。</li>
                <li>使用Vue在页面中完成数据的双向绑定,组件化开发。</li>
                <li>配合后台相关人员，实现网站的动态交互效果。以及接口文档的编写</li>
                <li>熟悉当下的各种流行库和框架及工具。</li>
                <li>有大型互联网项目开发经验，多人协作开发经验，常驻pC/移动端开发</li>
                <li>完。</li>
              </ul>
            </div>
          </div>
        </div>
        <v-footer></v-footer>
      </div>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
  import Footer from '@/components/footer'
  import Navigation from '@/components/navigation'

  export default {
    data () {
      return {
        show: false
      }
    },
    components: {
      'v-footer': Footer,
      Navigation
    }
  }
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
  .me
    position:relative
    min-height:100%
    margin:0
    padding:0
    background: #dee3e7
    &.detail
      height: 100%
      overflow: hidden
    .page
      padding-bottom: 45px
      overflow: hidden
      width: 100%
      .blog-detail
        padding: 0
        background: #dee3e7
        min-height: 100%
        .blog-detail-contaner
          max-width: 1000px
          margin: 0 auto
          background: #fff
          .header
            position: relative
            padding-top: 55%
            background-color: #eee
            background-size: cover
            background-position: 50%
            .header-cover
              position: absolute
              width: 100%
              height: 100%
              top: 0
              left: 0
              overflow: hidden
              text-align: center
              &.no-cover
                background: #1f3747
                background-image: -webkit-linear-gradient(left,#1f3747,#293d31)
              .header-body
                display: block
                margin-top: 20px
                .avatar
                  img
                    width: 120px
                    height: 120px
                    overflow: hidden
                    border-radius: 50%
                    background: $color-background
                    box-shadow: rgba(255, 255, 255, 0.1) 0 0 0 5px, rgba(0, 0, 0, 0.15) 0 0 5px 4px
                    transition: transform .4s ease-out
                  img:hover
                    transform: rotate(360deg)
                .tit
                  margin-top: 15px
                  line-height: 1.2
                  font-size: 26px
                  font-weight: 500
                  color: #fff
          .article-section
            padding: 1em 0
            .caption
              padding: 0 20px
              .titl
                margin-bottom: .4em
                font-size: 1.8rem
              .time
                font-size: 14px
            .article
              padding: 40px 20px
              font-size: 15px
              background: #fff
              &.markdown-body
                line-height: 1.5
                color: #24292e
                font-size: 16px
                font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
              ul
                padding-left: 2em
                li
                  &:before
                    position: absolute
                    left: 2.2em
                    width: 7px
                    height: 7px
                    background-color: #111
                    border-radius: 3.5px
                    content: ""
                    margin-top: 8px
                li+li
                  margin-top: 0.25em
              &:before
                display: table
                content: ""
</style>
