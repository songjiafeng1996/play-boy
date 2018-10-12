<template>
  <div id="app">
    <div class="nav-top">
      <div class="nav-top-left">
        <router-link to="">
          <div class="movie-first-stop fl">
            <img src="./assets/images/logo.png" alt="">
          </div>
        </router-link>
        <router-link to="">
          <div class="movie top-com fl">
            <span>电影</span>
          </div>
        </router-link>
        <router-link to="">
          <div class="TV-play top-com fl">
            <span>电视剧</span>
          </div>
        </router-link>
        <router-link to="">
          <div class="Comic top-com fl">
            <span>动漫</span>
          </div>
        </router-link>
        <router-link to="">
          <div class="nineth-area top-com fl">
            <span>第九区</span>
          </div>
        </router-link>
        <router-link to="">
          <div class="forest top-com fl">
            <span>小森林</span>
          </div>
        </router-link>
        <router-link to="">
          <div class="more top-com fl">
            <span>更多</span>
          </div>
        </router-link>
      </div>
      <div class="nav-top-right">
        <router-link to="">
          <span class="register fr">注册</span>
        </router-link>
        <router-link to="">
          <span class="login fr">登录</span>
        </router-link>
        <div class="search-box fr">
          <input type="text" class="search">
          <div class="btn-search">搜索</div>
        </div>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<script>

export default {
  name: "app",
};
</script>

<style lang="scss">
a{
  color:#fff;
}
html,body{
  background-color: #840308;
}
#app {
  width: 100%;

  .nav-top {
    height: 42px;
    width: 100%;
    background-color: #ff6666;
    font-size: 14px;
    color: #fff;
    .nav-top-left {
      width:650px;
      float: left;
      .movie-first-stop {
        height: 42px;
        width: 120px;
        margin-left: 2%;
      }
      .top-com {
        width: 73px;
        height: 42px;
        background: url("./assets/images/i3.png") 10px 10px no-repeat;
        line-height: 42px;
        span {
          padding-left: 35px;
        }
      }
      .TV-play {
        width: 88px;
        background: url("./assets/images/i3.png") 10px -30px no-repeat;
      }
      .Comic {
        background: url("./assets/images/i3.png") 10px -70px no-repeat;
      }
      .nineth-area {
        width:90px;
        background: url("./assets/images/i3.png") 10px -310px no-repeat;
      }
      .forest {
        width: 88px;
        background: url("./assets/images/i3.png") 10px -190px no-repeat;
      }
      .more {
        width:100px;
        background: url("./assets/images/i3.png") 10px -148px no-repeat;
      }
    }
    .nav-top-right {
      float: right;
      height: 42px;
      margin-right:30px;
      // line-height: 42px;
      .register {
         padding:0 10px;
         height: 18px;
         margin-top:12px;
         border-left:1px solid #c1c1c1;
      }
      .login{
        margin-top:12px;
         padding:0 10px;
      }
      .search-box{
        width:192px;
        height: 30px;
        border:1px solid #6cb5f4;
        margin-top:5px;
        .search{
         width:142px;
         height: 28px;
         float: left;
        }
        .btn-search{
          width:46px;
          height: 30px;
          background-color: #6cb5f4;
          color:#fff;
          line-height: 28px;
          text-align:center;
          float: left;
        }
      }
    }
  }
}
</style>
