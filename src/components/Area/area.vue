<template>
  <div id="area">
    <div class="inner">
      <div class="header">
        <p class="title">
          <span v-if="!reversal">
            {{title}}
            <span class="active">{{activeTitle}}</span>
          </span>
          <span v-if="reversal">
            <span class="active">{{activeTitle}}</span>
            {{title}}
          </span>
          <img class="img" src="@/assets/images/icons/camera.png" alt />
        </p>
        <p class="sub-title">{{subTitle}}</p>
      </div>
      <div class="center">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'navbar',
  data () {
    return {
      activeIndex: 'home',
    }
  },
  props: ['img', 'title', 'activeTitle', 'subTitle', 'reversal']

}
</script>

<style scoped lang="less">
@import url("../../assets/base.less");
.inner {
  margin: 0 auto;
  width: @base-width;
}
#area {
  padding-top: 70px;
}
.header {
  border-bottom: 1px solid #eaeaea;
  padding-bottom: 10px;
  margin-bottom: 50px;
  text-align: center;
  .title {
    font-size: 28px;
    font-weight: bold;
    color: rgba(0, 0, 0, 1);
    .active {
      font-size: 38px;
      font-weight: normal;
      color: rgba(194, 27, 31, 1);
    }
  }
  .sub-title {
    font-size: 16px;
    font-weight: 400;
    color: rgba(189, 189, 189, 1);
  }
  .img {
    vertical-align: middle;
    margin-left: 7px;
  }
}
</style>
