<template>
  <div class="infomation">
    <div class="profile">
      <h3>个人信息</h3>
      <div class="profile-item" v-for="item in profile">
        <span class="item-name">{{item.name}}</span>:<span class="item-content">{{item.content}}</span>
      </div>
    </div>
    <div class="contact">
      <h3>联系方式</h3>
      <div class="contact-item" v-for="item in contacts">
        <span class="item-name">{{item.name}}</span>:<span class="item-content">{{item.content}}</span>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'infomation',
    data () {
      return {
        contacts: [
          {name:'qq',content:'276906634'},
          {name:'微信',content:'16620460451'},
          {name:'电话',content:'16620460451'},
          {name:'e-mail',content:'caoxuxuan1992@QQ.com'}
        ],
        profile: [
          {name:'年龄',content:'27'},
          {name:'学历',content:'本科'},
          {name:'github',content:'https://github.com/cxxxingxuan'}
        ]
      }
    }

  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .infomation{
    h3{
      color: #4a9ac9;
    }
    .profile,
    .contact{
      border-bottom: 2px solid #c8c8ca;
      padding-bottom: 24px;
    }
    .profile-item,
    .contact-item{
      color: #b0b0b2;
      margin-bottom: 8px;
      .item-name{
        width: 72px;
        display: inline-block;
      }
      .item-content{
        display: inline-block;
        margin-left: 16px;
      }
    }
  }
</style>
