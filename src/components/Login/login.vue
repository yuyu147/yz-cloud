<template>
  <div id="login-card">
    <div class="login-inner clearfix">
      <div class="tab-header">
        <router-link to="/register" href>账号注册</router-link>
        <router-link class="active" to="/login" href>直接登录</router-link>
      </div>
      <div class="tab-content">
        <el-input class="form-input" placeholder="请输入账号" prefix-icon="el-icon-user-solid"></el-input>
        <el-input class="form-input" placeholder="请输入密码" prefix-icon="el-icon-s-goods"></el-input>
      </div>
      <div class="tab-bottom">
        <button class="up">登陆</button>
        <a class="bottom-link" href>忘记密码</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'login',
  data () {
    return {

    }
  }
}
</script>

<style scoped lang="less">
@import url("../../assets/base.less");
.active {
  color: #e30005;
}
#login-card {
  width: @base-width;
  margin: 0 auto;
  position: relative;
}
.login-inner {
  padding: 100px 25px 0 25px;
  box-sizing: border-box;
  width: 405px;
  height: 524px;
  background: rgba(255, 255, 255, 1);
  position: absolute;
  top: 38px;
  right: 0px;
  text-align: center;
}

.tab-header {
  display: flex;
  justify-content: space-between;
  font-size: 20px;
  color: rgba(136, 136, 136, 1);
  padding: 0 20px;
}

.tab-content {
  margin: 40px 0 30px 0;
  .form-input:last-of-type {
    margin-bottom: 0px;
  }
  .form-input {
    width: 300px;
    height: 40px;
    background: rgba(245, 250, 255, 1);
    border: 1px solid rgba(221, 221, 221, 1);
    border-radius: 5px;
    margin-bottom: 26px;
    font-size: 16px;
    font-weight: 400;
    color: rgba(102, 102, 102, 1);
  }
}
.tab-bottom {
  text-align: right;
  .up {
    margin-bottom: 30px;
    width: 100%;
    height: 48px;
    background: rgba(227, 0, 5, 1);
    border-radius: 4px;

    font-size: 16px;
    font-family: MicrosoftYaHei;
    font-weight: 400;
    color: rgba(255, 255, 255, 1);
  }
}
</style>
