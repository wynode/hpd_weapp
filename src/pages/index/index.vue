<template>
  <div>
    <div class="home_top">
      <image
        class="home_top_img"
        src="/static/images/首页icon/icon-sy-ad@3x.png"
      ></image>
      <div class="home_top_ab">
        <div class="hta_left">
          <image
            class="hta_location"
            src="/static/images/首页icon/icon-sy-address@3x.png"
          />
          <text class="hta_text">上海</text>
          <image
            class="hta_bottom"
            src="/static/images/首页icon/icon-sy-bottom@3x.png"
          />
        </div>

        <van-search
          class="hta_search"
          left-icon="/static/images/首页icon/icon-sy-search@3x.png"
          shape="round"
          placeholder="输入意向位置/业态"
        />
      </div>
    </div>
    <div class="home_s1">
      <div class="home_s1_left"></div>
      <div class="home_s1_right"></div>
    </div>
    <div class="home_s2">
      <div v-for="item in s2List" :key="item" class="home_s2_item">
        <image :src="item.url" class="home_s2_img"></image>
        <text class="home_s2_text">{{ item.name }}</text>
      </div>
    </div>
    <div class="home_s3">
      <image src="/static/images/首页icon/icon-sy-ad2@3x.png" class="home_s3_img"></image>
      <image src="/static/images/首页icon/icon-sy-ad1@3x.png" class="home_s3_img"></image>
    </div>
    <div class="home_s4">
      <image src="/static/images/首页icon/icon-sy-tt@3x.png" class="home_s4_img"></image>
      <div class="home_s4_right">
        <text>恭喜尾号8888顾客购买好铺多客户会员服务；恭喜尾号6666顾客购买好铺多房东会员服务；</text>
        <text>恭喜尾号8888顾客购买好铺多客户会员服务；恭喜尾号6666顾客购买好铺多房东会员服务；</text>
      </div>
    </div>
    <div class="home_s5">
      <image src="/static/images/首页icon/icon-sy-ad-kthy@3x.png" class="home_s5_img"></image>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      s2List: [
        {
          url: '/static/images/首页icon/icon-sy-zd@3x.png',
          name: '转店服务',
        },
        {
          url: '/static/images/首页icon/icon-sy-zdfw@3x.png',
          name: '找店服务',
        },
        {
          url: '/static/images/首页icon/icon-sy-xz@3x.png',
          name: '闲置物品',
        },
        {
          url: '/static/images/首页icon/icon-sy-pp@3x.png',
          name: '品牌合作',
        },
        {
          url: '/static/images/首页icon/icon-sy-zx@3x.png',
          name: '装修',
        },
      ],
    };
  },

  methods: {
    bindViewTap() {
      const url = "../logs/main";
      if (mpvuePlatform === "wx") {
        mpvue.switchTab({ url });
      } else {
        mpvue.navigateTo({ url });
      }
    },
  },
};
</script>

<style>
.home_top {
  height: 364px;
  width: 100%;
  position: relative;
}
.home_top_img {
  width: 100%;
  height: 364px;
}
.home_top_ab {
  position: absolute;
  display: flex;
  top: 0;
  left: 0;
  height: 74px;
  width: 100%;
  align-items: center;
}
.hta_left {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 130px;
  margin-left: 32px;
  margin-right: 32px;
}
.hta_text {
  color: #fff;
}
.hta_location {
  width: 24px;
  height: 30px;
}
.hta_bottom {
  width: 19px;
  height: 10px;
}
.hta_search {
  width: 522px;
}
.home_top_ab .van-search {
  padding: 0;
  border-radius: 40px;
}
.home_s1 {
  margin-top: 12px;
  margin-bottom: 38px;
  display: flex;
  justify-content: center;
}
.home_s1_left {
  width: 19px;
  height: 10px;
  background: #EC514E;
}
.home_s1_right{
  width: 19px;
  height: 10px;
  margin-left: 8px;
  background: #F9CACA;
}
.home_s2 {
  width: 670px;
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
}
.home_s2_img {
  width: 98px;
  height: 98px;
}
.home_s2_item {
  width: 98px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.home_s2_text {
  font-size: 22px;
  margin-top: 16px;
}
.home_s3 {
  width: 670px;
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
  margin-top: 43px;
}
.home_s3_img {
  width: 322px;
  height: 182px;
}
.home_s4 {
  width: 650px;
  display: flex;
  margin: 0 auto;
  margin-top: 36px;
}
.home_s4_img {
  width: 62px;
  height: 54px;
}
.home_s4_right {
  margin-left: 12px;
  line-height: 1.5;
  display: flex;
  flex-direction: column;
  color: #ADADAD;
  font-size: 14px;
  justify-content: center;
}
.home_s5 {
  width: 670px;
  height: 183px;
  margin: 0 auto;
  margin-top: 24px;
}
.home_s5_img {
  width: 670px;
  height: 183px;
}
</style>
