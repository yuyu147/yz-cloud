<template>
  <div id="header-top">
    <div class="inner">
      <div class="left">
        <a class="nav-link-left" href="#">登陆</a>
        <a href="#">注册</a>
      </div>
      <div class="right">
        <a class="nav-link-right" href="#">个人中心版</a>
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
