<template>
  <div id="login">
    <div class="inner clearfix">
      <div class="text">
        <p class="en-text">
          NEW ERA CIVILIZATION
          PRACTICE CENTER
        </p>
        <p class="heng"></p>
        <p class="cn-text">
          新时代
          <br />文明实践中心
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'login',
  data () { }
}
</script>

<style scoped lang="less">
@import url("../../assets/base.less");
#login {
  height: 600px;
  width: 100%;
  background: url("../../assets/images/login-bg.jpg") center no-repeat;
  background-size: cover;
  margin-top: 20px;
  position: relative;
}
.inner {
  .heng {
    height: 2px;
    width: 137px;
    height: 2px;
    background: rgba(255, 255, 255, 1);
    margin: 10px 0 15px 0;
  }
  .text {
    position: absolute;
    top: 45%;
    transform: translate(0, -50%);
  }
  margin: 0 auto;
  width: @base-width;
  .en-text {
    width: 700px;
  }
  .cn-text {
    width: 400px;
  }
  .en-text,
  .cn-text {
    font-size: 51px;
    font-weight: bold;
    color: rgba(255, 255, 255, 1);
    // line-height: 53px;
  }
}
</style>
