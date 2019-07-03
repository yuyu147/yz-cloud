<template>
  <div id="header-search">
    <div class="inner clearfix">
      <div class="right">
        <el-input
          class="search-input"
          placeholder="请输入要搜索的内容"
          suffix-icon="el-icon-search"
          v-model="search"
        ></el-input>
        <button class="search-btn">发布需求</button>
      </div>
      <div class="left">
        <img src="../../assets/logo.png" alt />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'search',
  data () {
    return {
      search: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
@import url("../../assets/base.less");
#header-search {
  .inner {
    width: @base-width;
    margin: 0 auto;
  }
  .right {
    float: right;
    transform: translate(0, 55%);
  }
  .left {
    float: left;
  }
}
.search-input {
  width: 427px;
  border-radius: 10px;
  /deep/ .el-input__inner {
    width: 427px;
    height: 56px;
    border: 2px solid rgba(194, 27, 31, 1);
    border-radius: 10px;
    font-size: 20px;
    color: rgba(164, 164, 164, 1);
    // line-height:52px;
  }
  /deep/ .el-input__icon {
    font-size: 20px;
  }
}

.search-btn {
  width: 189px;
  height: 55px;
  background: rgba(227, 0, 5, 1);
  border-radius: 10px;
  font-size: 20px;
  color: rgba(255, 255, 255, 1);
  margin-left: 18px;
  // line-height: 52px;
}
</style>
