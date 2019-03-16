<template>
  <div id="app">
    <div class="wrap">
      <header id="header">
        <div class="portrait"><img src="./assets/portrait.png"></div>
        <div class="name-job">
          <h1>曹谞轩</h1>
          <p>应聘Web前端开发</p>
        </div>

      </header>
      <container id="container">
        <aside>
          <Infomation/>
          <Skill/>
        </aside>
        <content>
          <Project/>
        </content>
      </container>
      <footer id="footer">
      </footer>
    </div>
  </div>
</template>

<script>
import Infomation from './components/infomation'
import Project from './components/project'
import Skill from './components/skill'

export default {
  name: 'app',
  components: {
    Infomation,
    Project,
    Skill
  }
}
</script>

<style lang="scss">
#app {
  font-family: "Microsoft YaHei",微软雅黑,"MicrosoftJhengHei",华文细黑,STHeiti,MingLiu;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #e6e7e9;
  .wrap{
    width: 950px;
    margin: 0 auto;
    background-color: #fff;
    #header{
      background-color: #3c3c3e;
      height: 250px;
      display: flex;
      .portrait{
        width: 200px;
        height: 200px;
        border-radius: 50%;
        margin: 25px;
        overflow: hidden;
        img{
          height: 100%;
          width: 100%;
        }
      }
      .name-job{
        flex: 1;
        margin-top: 75px;
        h1{
          color: #fdfdfd;
          font-size: 32px;
        }
        p{
          color: #6e6e70;
          font-size: 24px;
        }
      }
    }
    #container{
      background-color: #fff;
      text-align: left;
      display: flex;
      aside{
        width: 360px;
        padding: 16px;
        border-right: 2px solid #c8c8ca;
      }
      content{
        flex: 1;
        padding: 22px;
      }
    }
    #footer{
      height: 24px;
      background-color: #3c3c3e;
    }
  }
}

</style>
