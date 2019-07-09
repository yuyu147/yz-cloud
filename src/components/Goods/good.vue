<template>
  <div id="good">
    <img class="img" src="../../assets/images/good.png" alt />
    <div class="center">
      <p class="title">姓名：上官秀儿</p>
      <p class="sub-title">性别：女</p>
      <p class="service">已服务235.0小时</p>
      <div class="bottom">
        <el-rate class="star" v-model="rate" disabled text-color="#ff9900"></el-rate>
        <button class="subscribe">预约</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'good',
  data () {
    return {
      rate: 3
    }
  }
}
</script>

<style scoped lang="less">
@import url("../../assets/base.less");
#good {
  height: 453px;
  width: 285px;
  .img {
    width: 286px;
    height: 285px;
    vertical-align: middle;
  }
  .center {
    height: 169px;
    width: 100%;
    background-color: #f2f2f2;
    padding: 0 30px;
    box-sizing: border-box;
    padding-top: 17px;
    .title {
      font-size: 18px;
      font-weight: normal;
      color: rgba(52, 52, 52, 1);
      line-height: 30px;
    }
    .sub-title,
    .service {
      font-size: 16px;
      font-weight: normal;
      color: rgba(52, 52, 52, 1);
      line-height: 30px;
    }
    .bottom {
      border-top: 1px solid #e6e6e6;
      padding-top: 10px;
      .star {
        float: left;
      }
      /deep/.star .el-rate__icon {
        font-size: 28px;
        margin-right: 0px;
      }
      .subscribe {
        float: right;
        width: 67px;
        height: 33px;
        border: 1px solid rgba(217, 217, 217, 1);
        background-color: @base-color;
        border-radius: 15px;
        color: #fff;
      }
    }
  }
}
</style>
