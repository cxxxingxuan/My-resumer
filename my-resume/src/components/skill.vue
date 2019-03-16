<template>
  <div class="skill">
    <h3>个人技能</h3>
    <div class="skill-item">熟练 <span class="content-bold">HTML、DIV + CSS</span> 的页面布局，能根据设计图<span class="content-bold">像素级</span>完成页面制作</div>
    <div class="skill-item">熟悉 <span class="content-bold">HTML 5 及语义化，掌握 CSS 3 动画、过渡效果</span>等常用技术</div>
    <div class="skill-item">熟悉 <span class="content-bold">原生JavaScript</span>，会使用 <span class="content-bold">ES6+ 常用规范</span>，了解 <span class="content-bold">jQuery 常用 API 及思想</span></div>
    <div class="skill-item">熟悉 <span class="content-bold">Vue 常用功能</span>，理解如 <span class="content-bold">组件、虚拟 DOM、双向绑定</span>等概念，能够使用 <span class="content-bold">Vue 全家桶</span> 开发项目</div>
    <div class="skill-item">熟悉 <span class="content-bold">模块化、工程化</span>开发流程，能够 <span class="content-bold">配置 Webpack</span></div>
    <div class="skill-item">了解 <span class="content-bold">HTTP</span> 相关知识，了解常见的 <span class="content-bold">Web 性能优化方案</span></div>
    <div class="skill-item">熟练使用 <span class="content-bold">WebStorm、Sass、Git</span> 等开发工具</div>
  </div>

</template>

<script>
  export default {
    name: 'skill'
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.skill{
  h3{
    color: #4a9ac9;
  }
  .skill-item{
    color: #b0b0b2;
    margin-bottom: 8px;
    .content-bold{
      font-weight: bold;
      color: #1e2735;
    }
  }
}
</style>
