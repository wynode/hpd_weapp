<template>
  <div v-if="showkaipin" class="kaipin">
    <img src="http://wynode.com/haopuduo/开屏icon/icon-kaiping@3x.png" alt="">
  </div>
  <div v-else>
    <div class="home_top">
      <image class="home_top_img" src="http://wynode.com/haopuduo/首页icon/icon-sy-ad@3x.png"></image>
      <div class="home_top_ab">
        <div class="hta_left">
          <image class="hta_location" src="http://wynode.com/haopuduo/首页icon/icon-sy-address@3x.png" />
          <text class="hta_text">上海</text>
          <image class="hta_bottom" src="http://wynode.com/haopuduo/首页icon/icon-sy-bottom@3x.png" />
        </div>
        <van-search class="hta_search" left-icon="http://wynode.com/haopuduo/首页icon/icon-sy-search@3x.png" shape="round" placeholder="输入意向位置/业态" />
      </div>
    </div>
    <div class="home_s1">
      <div class="home_s1_left"></div>
      <div class="home_s1_right"></div>
    </div>
    <div class="home_s2">
      <div class="home_s2_item" @click="gozhuandian">
        <image src="http://wynode.com/haopuduo/首页icon/icon-sy-zd@3x.png" class="home_s2_img"></image>
        <text class="home_s2_text">转店服务</text>
      </div>
      <div class="home_s2_item" @click="gozhaodian">
        <image src="http://wynode.com/haopuduo/首页icon/icon-sy-zdfw@3x.png" class="home_s2_img"></image>
        <text class="home_s2_text">找店服务</text>
      </div>
      <div class="home_s2_item">
        <image src="http://wynode.com/haopuduo/首页icon/icon-sy-xz@3x.png" class="home_s2_img"></image>
        <text class="home_s2_text">闲置物品</text>
      </div>
      <div class="home_s2_item" @click="gohezuo">
        <image src="http://wynode.com/haopuduo/首页icon/icon-sy-pp@3x.png" class="home_s2_img"></image>
        <text class="home_s2_text">品牌合作</text>
      </div>
      <div class="home_s2_item">
        <image src="http://wynode.com/haopuduo/首页icon/icon-sy-zx@3x.png" class="home_s2_img"></image>
        <text class="home_s2_text">装修</text>
      </div>
    </div>
    <div class="home_s3">
      <image src="http://wynode.com/haopuduo/首页icon/icon-sy-ad2@3x.png" class="home_s3_img"></image>
      <image src="http://wynode.com/haopuduo/首页icon/icon-sy-ad1@3x.png" class="home_s3_img"></image>
    </div>
    <div class="home_s4">
      <image src="http://wynode.com/haopuduo/首页icon/icon-sy-tt@3x.png" class="home_s4_img"></image>
      <div class="home_s4_right">
        <p>恭喜尾号8888顾客购买好铺多客户会员服务；恭喜尾号6666顾客购买好铺多房东会员服务；</p>
        <p>恭喜尾号8888顾客购买好铺多客户会员服务；恭喜尾号6666顾客购买好铺多房东会员服务；</p>
      </div>
    </div>
    <div class="home_s5" @click="gokaitong">
      <image src="http://wynode.com/haopuduo/首页icon/icon-sy-ad-kthy@3x.png" class="home_s5_img"></image>
    </div>
    <div class="home_s6">
      <title :title="'好铺多精选'"></title>
      <div class="home_s6_content">
        <div class="home_s6_card1" @click="goshangpuxiangqin">
          <card :tagContent="'百货/购物中心'"></card>
        </div>
        <div class="home_s6_card2" @click="goshangpuxiangqin">
          <card imgUrl="http://wynode.com/haopuduo/首页icon/card2.png"></card>
        </div>
      </div>
    </div>
    <div class="home_s7">
      <title :title="'餐饮美食专题'"></title>
      <div class="home_s7_content" @click="goshangpuxiangqin">
        <img src="http://wynode.com/haopuduo/首页icon/card3.jpg" alt="" class="hs7c_img" />
        <img src="http://wynode.com/haopuduo/首页icon/icon-sy-cyms-tj@3x.png" alt="" class="hs7c_img2" />
        <div class="hs7c_info">
          店主自述：店铺位于顺义区鑫顺北大街，面积45平方，配套设施齐全，临街...
          <span class="hs7c_go">查看详情
            <img
              src="http://wynode.com/haopuduo/首页icon/icon-sy-cyms-go@3x.png"
              alt=""
              class="hs7c_img3"
            />
          </span>
        </div>
      </div>
    </div>
    <div class="home_s8">
      <title :title="'便利超市专题'"></title>
      <div class="home_s8_content" @click="goshangpuxiangqin">
        <seccard></seccard>
      </div>
    </div>
    <div class="home_s9" @click="gopuyuan">
      <img src="http://wynode.com/haopuduo/首页icon/icon-sy-cksp@3x.png" alt="" class="home_s9_img" />
    </div>
    <div class="home_s10">
      <title :title="'转店选址顾问'"></title>
      <div class="home_s10_content">
        <div class="hs10_top">
          <img src="http://wynode.com/haopuduo/首页icon/renwu.jpg" alt="" />
          <img src="http://wynode.com/haopuduo/首页icon/renwu.jpg" alt="" />
          <img src="http://wynode.com/haopuduo/首页icon/renwu.jpg" alt="" />
          <img src="http://wynode.com/haopuduo/首页icon/renwu.jpg" alt="" />
        </div>
        <div class="hs10_bottom">
          <img src="http://wynode.com/haopuduo/首页icon/icon-sy-zdxz-bg@3x.png" alt="" class="hs10_bottom_img" />
          <div class="hs10_bottom_content">
            <div class="hs10_text1">石跃军</div>
            <div class="hs10_text">
              擅长行业：<span>休闲娱乐，服装鞋包，百货超市</span>
            </div>
            <div class="hs10_text">服务过的人数：<span>2385人</span></div>
            <div class="hs10_ck">
              查看详情
              <img src="http://wynode.com/haopuduo/首页icon/icon-sy-cyms-go@3x.png" alt="" class="hs7c_img3" />
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="home_s11">
      <title :title="'品牌合作'"></title>
      <div class="home_s11_content">
        <div>
          <img src="http://wynode.com/haopuduo/首页icon/waipo.jpg" alt="" />
        </div>
        <div>
          <img src="http://wynode.com/haopuduo/首页icon/xibei.jpg" alt="" />
        </div>
        <div>
          <img src="http://wynode.com/haopuduo/首页icon/haidilao.jpg" alt="" />
        </div>
        <div>
          <img src="http://wynode.com/haopuduo/首页icon/xibei.jpg" alt="" />
        </div>
      </div>
    </div>
    <div class="home_s12">
      <title :title="'成交案例'"></title>
      <div class="home_s12_content">
        <div>
          <img src="http://wynode.com/haopuduo/首页icon/meinv.jpg" alt="" />
          <p>30天快速开店，好铺多助力王先生快速开店</p>
        </div>
        <div>
          <img src="http://wynode.com/haopuduo/首页icon/meinv.jpg" alt="" />
          <p>30天快速开店，好铺多助力王先生快速开店</p>
        </div>
      </div>
    </div>
    <div class="home_s13">
      <title :title="'猜你喜欢'" :showMore="false"></title>
      <div class="home_s13_content" @click="goshangpuxiangqin">
        <secitem v-for="item in 10" :key="item"></secitem>
      </div>
    </div>
  </div>
</template>

<script>
  import title from "@/components/title";
  import card from "@/components/card";
  import seccard from "@/components/seccard";
  import secitem from "@/components/secitem";
  export default {
    components: {
      title,
      card,
      seccard,
      secitem
    },
    data() {
      return {
        showkaipin: true,
      };
    },
    methods: {
      gozhuandian() {
        const url = "/pages/zhuandian/main";
        mpvue.navigateTo({
          url
        });
      },
      gozhaodian() {
        const url = "/pages/zhaodian/main";
        mpvue.navigateTo({
          url
        });
      },
      gohezuo() {
        const url = "/pages/hezuo/main";
        mpvue.navigateTo({
          url
        });
      },
      gopuyuan() {
        const url = "/pages/puyuan/main";
        wx.switchTab({
          url
        })
      },
      goshangpuxiangqin() {
        const url = "/pages/shangpuxiangqin/main";
        mpvue.navigateTo({
          url
        });
      },
      gokaitong() {
        const url = "/pages/kaitong/main";
        mpvue.navigateTo({
          url
        });
      }
    },
    mounted() {
      const that = this
      setTimeout(function() {
        that.showkaipin = false
      }, 3000);
    },
  };
</script>

<style>
  .kaipin {
    position: fixed;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    z-index: 1000;
  }
  .kaipin img {
    width: 100%;
    height: 100%;
  }
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
    background: #ec514e;
  }
  .home_s1_right {
    width: 19px;
    height: 10px;
    margin-left: 8px;
    background: #f9caca;
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
    color: #adadad;
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
  .home_s6 {
    width: 670px;
    margin: 0 auto;
    margin-top: 46px;
  }
  .home_s6_content {
    width: 670px;
    margin: 0 auto;
    margin-top: 23px;
    display: flex;
    justify-content: space-between;
  }
  .home_s6_card1 {
    width: 442px;
  }
  .home_s6_card2 {
    width: 214px;
  }
  .home_s7 {
    width: 670px;
    margin: 0 auto;
    margin-top: 34px;
  }
  .home_s7_content {
    width: 670px;
    height: 300px;
    margin: 0 auto;
    position: relative;
    margin-top: 23px;
    box-shadow: 0px 2px 4px 0px rgba(6, 0, 1, 0.2);
    border-radius: 6px;
    overflow: hidden;
  }
  .hs7c_img {
    width: 670px;
    height: 300px;
  }
  .hs7c_img2 {
    width: 88px;
    height: 89px;
    position: absolute;
    top: 0;
    right: 20px;
  }
  .hs7c_info {
    width: 670px;
    height: 76px;
    background: rgba(255, 255, 255, 0.7);
    color: #333333;
    box-sizing: border-box;
    padding: 14px;
    font-size: 20px;
    position: absolute;
    bottom: 0;
    left: 0;
  }
  .hs7c_img3 {
    margin-left: 4px;
    width: 9px;
    height: 16px;
  }
  .hs7c_go {
    color: #ec514e;
    margin-left: 6px;
  }
  .home_s8 {
    width: 670px;
    margin: 0 auto;
    margin-top: 46px;
  }
  .home_s8_content {
    margin-top: 15px;
  }
  .home_s9 {
    width: 670px;
    margin: 0 auto;
    margin-top: 38px;
  }
  .home_s9_img {
    width: 670px;
    height: 247px;
  }
  .home_s10 {
    width: 670px;
    margin: 0 auto;
    margin-top: 48px;
  }
  .home_s10_content {
    width: 670px;
    margin: 0 auto;
    margin-top: 36px;
  }
  .hs10_top {
    display: flex;
    justify-content: space-between;
  }
  .hs10_top img {
    width: 122px;
    height: 122px;
    border-radius: 50%;
  }
  .hs10_bottom {
    margin-top: 11px;
    position: relative;
    margin-left: 8px;
  }
  .hs10_bottom_img {
    width: 616px;
    height: 243px;
  }
  .hs10_bottom_content {
    padding-top: 38px;
    padding-left: 23px;
    position: absolute;
    left: 0;
    top: 0;
  }
  .hs10_text {
    color: #767676;
    margin-top: 6px;
    font-size: 24px;
  }
  .hs10_text1 {
    color: #1a1a1a;
  }
  .hs10_text span {
    color: #1a1a1a;
    font-size: 24px;
  }
  .hs10_ck {
    color: #ec514e;
    font-size: 24px;
    margin-top: 10px;
  }
  .home_s11 {
    width: 670px;
    margin: 0 auto;
    margin-top: 48px;
  }
  .home_s11_content {
    display: flex;
    justify-content: space-between;
    margin-top: 28px;
  }
  .home_s11_content div {
    width: 149px;
    height: 121px;
    display: flex;
    justify-content: center;
    align-items: center;
    box-shadow: 0px 2px 4px 0px rgba(6, 0, 1, 0.2);
    border-radius: 6px;
  }
  .home_s11_content div img {
    width: 114px;
    height: 70px;
  }
  .home_s12 {
    width: 670px;
    margin: 0 auto;
    margin-top: 38px;
  }
  .home_s12_content {
    display: flex;
    justify-content: space-between;
    margin-top: 18px;
  }
  .home_s12_content div {
    width: 310px;
    height: 314px;
    box-shadow: 0px 5px 6px 0px rgba(6, 0, 1, 0.2);
    border-radius: 6px;
  }
  .home_s12_content img {
    width: 310px;
    height: 190px;
  }
  .home_s12_content p {
    color: #1A1A1A;
    font-size: 28px;
    margin-top: 18px;
    margin-left: 12px;
  }
  .home_s13 {
    width: 690px;
    margin: 0 auto;
    margin-top: 38px;
  }
  .home_s13_content {
    width: 690px;
    margin: 0 auto;
  }
</style>
