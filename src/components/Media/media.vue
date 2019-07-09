<template>
  <div id="media">
    <div class="header">
      <div class="img">图片</div>
      <div class="title">防溺水保安全宣传活动（招募中）</div>
    </div>
    <div class="center">
      <p class="content">年降电费700亿 2018“新电改”红利仍将继续释放提不充分的问题进行了认真梳理特别是对分管财务的领导同志进行约谈。年降电费700亿 。</p>
      <p class="team">发起团体:任城区教育中心时代建设服务队</p>
      <p class="time">招募日期:2019.06.01-2019.07.04</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'media',
  data () {
    return {
    }
  }
}
</script>

<style scoped lang="less">
@import url("../../assets/base.less");
#media {
  margin: 0 auto;
  position: relative;
  display: inline-block;
  width: 447px;
}
.header {
  display: inline-block;
  margin-bottom: 10px;
  .img {
    display: inline-block;
    width: 65px;
    height: 65px;
    background-color: @base-color;
    border-radius: 50%;
    text-align: center;
    float: left;
  }
  .title {
    width: 391px;
    height: 65px;
    display: inline-block;

    font-size: 24px;
    font-weight: normal;
    color: rgba(255, 255, 255, 1);
    line-height: 64px;
    text-align: right;
    margin-left: -10px;
    position: relative;
    z-index: -1;
    background-image: radial-gradient(
      36px at -17px 32px,
      #fff 36px,
      @base-color 0
    );
  }
}
.center {
  width: 447px;
  height: 168px;
  background-color: #f9f9f9;
  display: inline-block;
  box-sizing: border-box;
  .team,
  .time {
    font-size: 16px;
    font-weight: 600;
    color: rgba(100, 100, 100, 1);
    line-height: 32px;
  }
  .content {
    text-indent: 2em;
    font-size: 16px;
    font-weight: 600;
    color: rgba(0, 0, 0, 1);
    line-height: 32px;
  }
}
</style>
