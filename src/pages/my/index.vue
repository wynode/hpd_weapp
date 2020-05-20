<template>
  <div class="my">
    <div class="my_top">
      <img src="http://wynode.com/haopuduo/我的icon/icon-wd-bg@3x.png" alt="" class="my_top_img" />
      <div class="my_top_content">
        <img src="http://wynode.com/haopuduo/我的icon/icon-wd-tx@3x.jpg" alt="" class="mtc_img" />
        <div class="mtc_center">
          <div class="mtc_center_top">用户ID：13711118888</div>
          <div class="mtc_center_bottom">
            <img src="http://wynode.com/haopuduo/我的icon/icon-wd-dqsj@3x.png" alt="" />
            <p>会员到期时间：2020年05月15日</p>
          </div>
        </div>
      </div>
      <div class="mtc_right">
        <img src="http://wynode.com/haopuduo/我的icon/icon-wd-yhxx@3x.png" alt="" />
        <p>用户信息 ></p>
      </div>
    </div>
    <div class="my_s1">
      <div class="my_s1_row">
        <div class="my_s1_item">
          <img src="http://wynode.com/haopuduo/我的icon/icon-wd-wy@3x.png" alt="" class="my_s1_img" />
          <p class="my_s1_p">我的物业</p>
        </div>
        <div class="my_s1_item">
          <img src="http://wynode.com/haopuduo/我的icon/icon-wd-xz@3x.png" alt="" class="my_s1_img" />
          <p class="my_s1_p">我的选址</p>
        </div>
        <div class="my_s1_item" @click="gozhuandian">
          <img src="http://wynode.com/haopuduo/我的icon/icon-wd-zr@3x.png" alt="" class="my_s1_img" />
          <p class="my_s1_p">物品转让</p>
        </div>
        <div class="my_s1_item">
          <img src="http://wynode.com/haopuduo/我的icon/icon-wd-sc@3x.png" alt="" class="my_s1_img" />
          <p class="my_s1_p">我的收藏</p>
        </div>
      </div>
      <div class="my_s1_row2">
        <div class="my_s1_item">
          <img src="http://wynode.com/haopuduo/我的icon/icon-wd-dy@3x.png" alt="" class="my_s1_img" />
          <p class="my_s1_p">我的订阅</p>
        </div>
        <div class="my_s1_item">
          <img src="http://wynode.com/haopuduo/我的icon/icon-wd-kf@3x.png" alt="" class="my_s1_img" />
          <p class="my_s1_p">联系客服</p>
        </div>
        <div class="my_s1_item" @click="gopaidian">
          <img src="http://wynode.com/haopuduo/我的icon/icon-wd-pd@3x.png" alt="" class="my_s1_img" />
          <p class="my_s1_p">拍店赚钱</p>
        </div>
      </div>
    </div>
    <div class="my_s2">
      <img src="http://wynode.com/haopuduo/我的icon/icon-wd-ad@3x.png" alt="" />
    </div>
    <div class="my_s3">
      <img src="http://wynode.com/haopuduo/我的icon/hpd.jpg" alt="" />
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {};
    },
    methods: {
      gopaidian() {
        const url = "/pages/paidian/main";
        mpvue.navigateTo({
          url
        });
      },
      gozhuandian() {
        const url = "/pages/zhuandian/main";
        mpvue.navigateTo({
          url
        });
      }
    },
  };
</script>

<style>
  .my {
    width: 100%;
  }
  .my_top {
    width: 100%;
  }
  .my_top_img {
    width: 100%;
    height: 210px;
  }
  .my_top_content {
    display: flex;
    position: absolute;
    top: 26px;
    left: 0px;
  }
  .mtc_img {
    width: 104px;
    height: 104px;
    margin-left: 20px;
    border-radius: 50%;
  }
  .mtc_center {
    margin-left: 26px;
  }
  .mtc_center_top {
    font-size: 30px;
    color: #fff;
    margin-top: 4px;
  }
  .mtc_center_bottom {
    position: relative;
    margin-top: 14px;
  }
  .mtc_center_bottom img {
    width: 270px;
    height: 35px;
  }
  .mtc_center_bottom p {
    position: absolute;
    color: #e93534;
    font-size: 16px;
    top: 6px;
    left: 20px;
  }
  .mtc_right {
    position: absolute;
    right: 0;
    top: 40px;
  }
  .mtc_right img {
    width: 94px;
    height: 30px;
  }
  .mtc_right p {
    position: absolute;
    left: 12px;
    top: 6px;
    font-size: 15px;
    color: #fff;
  }
  .my_s1 {
    width: 610px;
    height: 232px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    margin-top: 64px;
    margin-bottom: 76px;
  }
  .my_s1_row {
    display: flex;
    justify-content: space-between;
  }
  .my_s1_row2 {
    display: flex;
    justify-content: flex-start;
  }
  .my_s1_row2 div {
    margin-right: 70px;
  }
  .my_s1_item {
    width: 100px;
    height: 84px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
  }
  .my_s1_img {
    height: 40px;
    width: 40px;
  }
  .my_s1_p {
    font-size: 24px;
    color: #333333;
  }
  .my_s2 {
    width: 710px;
    margin: 0 auto;
  }
  .my_s2 img {
    width: 709px;
    height: 225px;
  }
  .my_s3 {
    width: 100px;
    margin: 0 auto;
    margin-top: 94px;
  }
  .my_s3 img {
    width: 100px;
    height: 68px;
  }
</style>
