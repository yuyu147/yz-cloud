<template>
  <div id="header-top">
    <div class="inner">
      <div class="left">
        <router-link class="nav-link-left" to="/login">登陆</router-link>
        <router-link class="nav-link-left" to="/register">注册</router-link>
      </div>
      <div class="right">
        <router-link class="nav-link-right" to="home">个人中心版</router-link>
        <a class="nav-link-right" href="#">免费发布信息</a>
        <a class="nav-link-right" href="#">APP下载</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'top'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
@import url("../../assets/base.less");
#header-top {
  width: 100%;
  height: 36px;
  background: rgba(220, 220, 220, 1);

  font-size: 17px;
  color: rgba(0, 0, 0, 1);
  line-height: 35px;
  .inner {
    width: @base-width;
    margin: 0 auto;
    .left {
      float: left;
    }
    .nav-link-left {
      padding-right: 25px;
    }
    .nav-link-right {
      padding-left: 25px;
    }
    .right {
      float: right;
    }
  }
}
</style>
