<template>
  <div id="footer">
    <div class="inner">
      <p class="s-link">
        <a href>首页</a>
        <span class="shu"></span>
        <a href>志愿者</a>
        <span class="shu"></span>
        <a href>志愿者团队</a>
        <span class="shu"></span>
        <a href>近期活动</a>
        <span class="shu"></span>
        <a href>便民中心</a>
        <span class="shu"></span>
        <a href>服务咨询</a>
      </p>
      <p class="copyright">Copyright © 2016-2017 中文 English</p>
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
#footer {
  text-align: center;
  height: 150px;
}
.s-link {
  margin-top: 50px;
}
.copyright {
  margin: 20px 0 50px 0;
}
.s-link,
.copyright {
  font-size: 18px;
  color: rgba(136, 136, 136, 1);
  a {
    color: rgba(136, 136, 136, 1);
  }
  .shu {
    height: 20px;
    background-color: rgba(136, 136, 136, 1);
    width: 1px;
    display: inline-block;
    vertical-align: middle;
    margin: 0 20px;
  }
}
</style>
