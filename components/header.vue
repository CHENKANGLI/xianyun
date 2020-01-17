<template>
 <div class="header-wapper">
     <el-row class="header" type="flex" justify="space-between" align="middle">
      <div class="logo">
          <img src="/logo.jpg" alt="">
      </div>
     <el-row class="navs" type="flex" align="middle">
         <nuxt-link to="/">首页</nuxt-link>
         <nuxt-link to="/post">旅游攻略</nuxt-link>
         <nuxt-link to="/hotel">酒店</nuxt-link>
         <nuxt-link to="/air">国内机票</nuxt-link>
     </el-row>
      <div class="login">
         <nuxt-link to="/user">登录/注册</nuxt-link>
      </div>
  </el-row>
 </div>
</template>

<script>
export default {
 data () {
     return {
         current:0
     }
 }
}
</script>

<style lang='less' scoped>
  .header-wapper {
      height: 60px;
      border-bottom: 1px solid #ccc;
      box-shadow: 0 5px 3px #ccc;
  }
  .header {
      width: 1000px;
      height: 100%;
      margin: 0 auto;
      .logo {
          img {
              width: 156px;
              height: 42px;
          }
      }
      .navs {
          margin: 0 20px;
          flex: 1;
          a {
              display: block;
              height: 60px;
              line-height: 60px;
              padding: 0 20px;
              &:hover {
                  color: #409eff;
                  border-bottom: 5px solid #409eff;
              }
          }
          /deep/ .nuxt-link-exact-active{
                background:#409eff;
                color:#fff!important;
                :hover {
                  color: #fff;
              }
            }
      }
      .login {
          a {
              color: #666;
              font-size: 14px;
              &:hover {
                  color: #409eff;
              }
          }
      }
  }
</style>