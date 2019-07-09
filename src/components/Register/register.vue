<template>
  <div id="register-card">
    <div class="register-inner clearfix">
      <div class="tab-header">
        <router-link class="active" to="/register" href>账号注册</router-link>
        <router-link to="/login" href>直接登录</router-link>
      </div>
      <div class="tab-content">
        <el-input class="form-input" placeholder="请输入姓名" prefix-icon="el-icon-user-solid"></el-input>
        <el-input class="form-input" placeholder="请输入家庭住址" prefix-icon="el-icon-s-home"></el-input>
        <el-input class="form-input" placeholder="请输入手机号" prefix-icon="el-icon-phone"></el-input>
        <el-input class="form-input" placeholder="请输入验证码" prefix-icon="el-icon-phone"></el-input>
        <el-input class="form-input" placeholder="设置密码" prefix-icon="el-icon-s-goods"></el-input>
        <el-input class="form-input" placeholder="再次确认密码" prefix-icon="el-icon-s-goods"></el-input>
        <div class="agree">
          <el-checkbox label="city">同意《注册服务协议》</el-checkbox>
        </div>
      </div>
      <div class="tab-bottom">
        <button class="up">登陆</button>
        <a class="bottom-link" href>已有账户？马上登陆</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'register',
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
#register-card {
  width: @base-width;
  margin: 0 auto;
  position: relative;
}
.register-inner {
  padding: 25px 25px 0 25px;
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
  .agree {
    text-align: left;
    padding-left: 27px;
    padding-top: 17px;

    font-size: 14px;
    font-weight: 400;
    color: rgba(51, 51, 51, 1);
  }
  // text-align: left;
  margin: 40px 0 10px 0;
  .form-input:last-of-type {
    margin-bottom: 0px;
  }
  .form-input {
    /deep/ .el-input__inner {
      background: rgba(245, 250, 255, 1) !important;
    }
    width: 300px;
    height: 40px;
    border: 1px solid rgba(221, 221, 221, 1);
    border-radius: 5px;
    margin-bottom: 8px;
    font-size: 16px;
    font-weight: 400;
    color: rgba(102, 102, 102, 1);
  }
}
.tab-bottom {
  text-align: center;
  .up {
    margin-bottom: 8px;
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
