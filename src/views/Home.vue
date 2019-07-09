<template>
  <div id="home">
    <div class="banner">
      <div class="inner">
        <div class="classify">
          <p class="header">地区分类</p>
          <div class="center">
            <div class="line">
              <p class="sub-media-title">地区分类一</p>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
            </div>
            <div class="line">
              <p class="sub-media-title">地区分类一</p>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
            </div>
            <div class="line">
              <p class="sub-media-title">地区分类一</p>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
            </div>
            <div class="line">
              <p class="sub-media-title">地区分类一</p>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
            </div>
            <div class="line">
              <p class="sub-media-title">地区分类一</p>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
              <span class="item">分类一</span>
            </div>
            <div class="line-more">
              <span class="more">更多 >>></span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="center clearfix">
      <div id="active">
        <Area
          title="近期"
          subTitle="SOCIAL SERVICES"
          img="@/assets/images/icons/camera.png"
          activeTitle="活动"
        >
          <div class="left">
            <div class="media-title">
              <span>近期活动</span>
              <span class="fr more">更多 >>></span>
            </div>
            <div>
              <div class="media-line">
                <Media class="media" />
                <Media />
              </div>
              <div class="media-line">
                <Media class="media" />
                <Media />
              </div>
            </div>
          </div>
          <div class="right">
            <div class="active1">
              <img class="img" src="../assets/images/icons/arrows.png" alt />
              <span class="text1">最新活动</span>
              <span class="text2">Public opinion</span>
            </div>
            <div class="active2">
              <img class="img" src="../assets/images/icons/hammer.png" alt />
              <span class="text1">活动中心</span>
              <span class="text2">Complaint reporting</span>
            </div>
            <img class="avtice-img" src="../assets/images/active.png" alt />
            <img class="avtice-img" src="../assets/images/active.png" alt />
          </div>
        </Area>
      </div>
    </div>
    <div class="center clearfix">
      <div id="team">
        <Area
          title="志愿"
          subTitle="SPECIAL COLUMN"
          img="@/assets/images/icons/camera.png"
          activeTitle="团队"
          :reversal="true"
        >
          <!-- 团队内容 -->
          <div class="team-tab">
            <span class="tab-item">优秀志愿者</span>
            <span class="tab-item">志愿团队</span>
            <span class="tab-more">更多 >>></span>
          </div>
          <div class="team-center">
            <swiper :options="swiperOption">
              <swiper-slide v-for="i in 5" :key="i">
                <Good class="good" />
              </swiper-slide>
            </swiper>
            <div class="swiper-button-prev"></div>
            <!--左箭头。如果放置在swiper-container外面，需要自定义样式。-->
            <div class="swiper-button-next"></div>
            <!--右箭头。如果放置在swiper-container外面，需要自定义样式。-->
          </div>
        </Area>
      </div>
    </div>
    <div class="center clearfix">
      <div id="team">
        <Area
          title="服务"
          subTitle="PUBLIC PARTICIPATION IN"
          img="@/assets/images/icons/camera.png"
          activeTitle="资讯"
        >
          <div class="media-title">
            <span>近期活动</span>
            <span class="fr more">更多 >>></span>
          </div>
        </Area>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Area from '@/components/Area/area.vue'
import Media from '@/components/Media/media.vue'
import Good from '@/components/Goods/good.vue'
import { swiper, swiperSlide } from 'vue-awesome-swiper'

export default {
  name: 'home',
  components: { Area, Media, Good, swiper, swiperSlide },
  data () {
    return {
      swiperOption: {
        slidesPerView: 'auto',
        spaceBetween: -50,
        slidesPerView: 4,
        slidesPerGroup: 4,
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev',
        },
      }
    }
  }
}
methods: {

}
</script>

<style lang="less" scoped>
// @import url("../../node_modules/swiper/src/swiper.less");
@import url("../../node_modules/swiper/dist/css/swiper.css");

@import url("../assets/base.less");
/deep/ #media:first-of-type {
  margin-right: 16px;
}
.left {
  width: 910px;
  float: left;
}
/* 媒体标题 */
/deep/ .media-title {
  font-size: 22px;
  font-weight: normal;
  color: rgba(0, 0, 0, 1);
  line-height: 32px;
  border-left: 3px solid @base-color;
  padding-left: 10px;
  margin-bottom: 20px;
  .more {
    color: @base-color;
  }
}

/* 媒体 right */
.media-line:first-of-type {
  margin-bottom: 12px;
}
.right {
  width: 391px;
  float: right;
  .text1,
  .text2 {
    font-size: 24px;
    font-weight: normal;
    color: rgba(255, 255, 255, 1);
  }
  .text2 {
    font-size: 18px;
  }
  .active1 {
    position: relative;
    width: 100%;
    height: 150px;
    background-color: #e98031;
    .img {
      position: absolute;
      top: 54px;
      left: 94px;
    }
    .text1 {
      position: absolute;
      left: 195px;
      top: 46px;
    }
    .text2 {
      position: absolute;
      left: 195px;
      top: 90px;
    }
  }
  .avtice-img:first-of-type {
    padding-right: 9px;
  }
  .avtice-img {
    width: 191px;
    height: 229px;
  }
  .active2 {
    position: relative;
    width: 100%;
    height: 150px;
    margin: 10px 0px;
    background-color: #e49a37;
    .img {
      position: absolute;
      top: 54px;
      right: 75px;
    }
    .text1 {
      position: absolute;
      left: 50px;
      top: 46px;
    }
    .text2 {
      position: absolute;
      left: 50px;
      top: 90px;
    }
  }
}

.banner {
  background: url("../assets/images/banner.png") no-repeat center;
  background-size: 100% 100%;
  height: 750px;
  margin-top: 6px;
}
.classify {
  width: 483px;
  height: 618px;
  background: rgba(255, 255, 255, 1);
  opacity: 0.9;
  border-radius: 10px;
  .line-more {
    text-align: right;
    color: red;
    font-size: 18px;
  }
  .center {
    .line {
      margin-bottom: 30px;
    }
    padding: 36px 30px;
    .sub-media-title {
      font-size: 22px;
      font-weight: 600;
      color: rgba(70, 68, 89, 1);
      line-height: 32px;
    }
    .item {
      font-size: 20px;
      font-weight: 200;
      color: rgba(70, 68, 89, 1);
      line-height: 32px;
      padding-right: 30px;
    }
  }
  .header {
    height: 70px;
    line-height: 70px;
    text-align: center;
    font-size: 22px;
    font-weight: 600;
    background-origin: padding-box;
    border-bottom: 1px solid rgba(70, 68, 89, 1);
  }
}

// 团队支援
#team {
  .team-center {
    position: relative;
    // padding: 0 50px;
  }
  .good {
    box-sizing: border-box;
  }
  .tab-item {
    height: 42px;
    padding: 10px 15px;
    border: 1px solid rgba(194, 27, 31, 1);
    font-size: 20px;
    font-weight: 600;
    color: rgba(194, 27, 31, 1);
    margin-right: 40px;
  }
  .team-tab {
    padding-bottom: 35px;
  }
  .tab-more {
    float: right;
    font-size: 22px;
    font-weight: normal;
    color: rgba(194, 27, 31, 1);
  }
}
</style>
