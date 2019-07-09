<template>
  <div id="navbar">
    <el-menu
      :default-active="activeIndex"
      router
      class="el-menu-demo"
      mode="horizontal"
      active-text-color="#e30005"
      @select="handleSelect"
    >
      <el-menu-item index="home">首页</el-menu-item>
      <el-menu-item index="2">处理中心</el-menu-item>
      <el-menu-item index="3">消息中心</el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: 'navbar',
  data () {
    return {
      activeIndex: 'home',
    }
  }
}
</script>

<style scoped lang="less">
@import url("../../assets/base.less");
.active {
  color: #e30005;
}
#navbar {
  margin: 0 auto;
  position: relative;
  width: @base-width;
}
.el-menu-demo {
  border-bottom: solid 2px @base-color!important;
  /deep/ .el-menu-item {
    font-weight: 600;
    font-size: 22px;
    color: rgba(0, 0, 0, 1);
  }
  /deep/ .el-menu-item,
  .active {
    border-bottom: solid 0px @base-color!important;
  }
}
</style>
