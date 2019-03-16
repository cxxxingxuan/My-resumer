<template>
  <div class="project">
    <h3>项目经历</h3>
    <div class="project-item" v-for="project in projects">
      <div class="project-name">
        {{project.name}}
      </div>
      <div class="project-introduce">
        项目介绍:{{project.content}}
      </div>
      <div class="project-img">
        <img :src="project.img">
      </div>
      <div class="project-URL" >
        <a :href="project.URL">预览地址</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'project',
  data () {
    return {
      projects : [
        {name:'慕课教育动态宣传网页',content:'利用H5本地存储，css3阴影，css3动画，选择器等技术设计制作web页面',URL:'https://cxxxingxuan.github.io/imooc/',img: require('../assets/imooc.jpg')},
        {name:'可爱的海绵宝宝',content:'是一个使用纯原生 JS 开发的，动态显示 CSS 画一个皮卡丘过程的小作品。该作品主要思路是通过间隔计时器遍历预先设置在 preview 标签内代码，将其一个个显示在页面上，并在 style 标签上作同样处理，以使代码 CSS 生效。此外，也实现了调速功能。',URL:'https://cxxxingxuan.github.io/dynamicCSS/',img: require('../assets/dynamicCSS.png')},
        {name:'Vue简历编辑器',content:'使用Vue、VueX、Vue-router、LeanCloud编写一个简历编辑器，包裹在线保存、登录注册、预览简历等功能。',URL:'https://cxxxingxuan.github.io/My-project/dist/index.html#/',img: require('../assets/vueresume.png')}
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.project{
  h3 {
    color: #4a9ac9;
    margin-top: 8px;
  }
  .project-item{
    border-bottom: 1px solid #c8c8ca;
    margin-bottom: 16px;
    .project-name{
      font-weight: bold;
    }
    .project-introduce{
      margin-top: 8px;
    }
    .project-img{
      width: 380px;
      height: 160px;
      margin: 8px auto;
      img{
        width: 100%;
        height: 100%;
      }
    }
    .project-URL{
      margin-bottom: 8px;
    }
  }
}
</style>
