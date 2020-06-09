<template>
  <div class="spxq">
    <div class="spxq_top">
      <img v-if="activeimage" src="http://wynode.com/haopuduo/首页icon/room.jpg" alt="">
      <img v-else src="http://wynode.com/haopuduo/商铺详情icon/bg1.jpg" alt="">
      <div class="spxq_topx">
        <h2 @click="activeimage=false" :class="{ activebg: !activeimage }">视频</h2>
        <p @click="activeimage=true" :class="{ activebg: activeimage }">图片</p>
      </div>
    </div>
    <div class="spxq_s1">
      <h1>望海路软件园二期公寓低价转让</h1>
      <div class="spxq_s1_1">
        <p><img src="http://wynode.com/haopuduo/商铺详情icon/icon-shop-hot@3x.png" alt="">热门</p>
        <p>便利超市</p>
        <p>十字或拐角</p>
        <p>其他</p>
      </div>
      <div class="spxq_s1_2">
        <div>
          <p>面积（㎡）</p>
          <span>60</span>
        </div>
        <div>
          <p>租金（元/月）</p>
          <span>5800</span>
        </div>
        <div>
          <p>转让费（万元/月）</p>
          <span>面议</span>
        </div>
      </div>
    </div>
    <div class="spxq_s2">
      <div class="spxq_item">
        <p>区域：<span>鼓楼区-西洪路</span></p>
        <p>商圈：<span>金牛山</span></p>
      </div>
      <div class="spxq_item">
        <p>小区：<span>万隆花园一期</span></p>
        <p>面宽：<span>4米</span></p>
      </div>
      <div class="spxq_item">
        <p>进深：<span>4米</span></p>
        <p>层高：<span>4米</span></p>
      </div>
      <div class="spxq_item1">
        <p>地址：<span>鼓楼区西洪路457-2美华隆佳便利</span></p>
        <p>
          <img src="http://wynode.com/haopuduo/商铺详情icon/icon-shop-address@3x.png" alt="">
          <span class="spxq_item1_span">查看地图</span>
        </p>
      </div>
      <div class="spxq_item2">
        <p>地址：<span>望海路软件园二期公寓靠近地铁商超，周边交通便利，生活环境优越...</span></p>
      </div>
    </div>
    <div class="spxq_s3" @click="gokaitong">
      <img src="http://wynode.com/haopuduo/商铺详情icon/icon-shop-ad@3x.png" alt="">
    </div>
    <div class="spxq_s4">
      <h1>
        猜你喜欢
      </h1>
      <secitem v-for="item in 10" :key="item" :btntype="'default'"></secitem>
    </div>
    <div class="spxq_bottom">
      <div class="spxq_b1">
        <img src="http://wynode.com/haopuduo/商铺详情icon/icon-shop-wsc@3x.png" alt="" @click="showRed = true" v-if="!showRed">
        <img src="http://wynode.com/haopuduo/商铺详情icon/icon-shop-ysc@3x.png" alt="" @click="showRed = false" v-else>
        <p>收藏</p>
      </div>
      <div class="spxq_b2">
        <p>已租提醒</p>
      </div>
      <div class="spxq_b3">
        <p>直通房东</p>
      </div>
    </div>
  </div>
</template>

<script>
  import secitem from '@/components/secitem'
  export default {
    components: {
      secitem,
    },
    data() {
      return {
        showRed: false,
        activeimage: false,
      }
    },
    methods: {
      gokaitong() {
        const url = "/pages/kaitong/main";
        mpvue.navigateTo({
          url
        });
      }
    },
  }
</script>

<style lang="scss">
  .spxq {
    width: 710px;
    margin: 0 auto;
    .spxq_top {
      margin-top: 20px;
      position: relative;
      img {
        width: 710px;
        height: 316px;
      }
      .spxq_topx {
        display: flex;
        width: 168px;
        height: 42px;
        border-radius: 20px;
        position: absolute;
        left: 271px;
        bottom: 18px;
        text-align: center;
        background: #97999D;
        h2 {
          font-size: 22px;
          font-weight: 400;
          line-height: 42px;
          color: #fff;
          width: 85px;
          border-radius: 20px;
          height: 42px
        }
        p {
          font-size: 22px;
          font-weight: 400;
          line-height: 42px;
          color: #fff;
          width: 85px;
          border-radius: 20px;
          height: 42px
        }
        .activebg {
          background: #EC514E;
        }
      }
    }
    .spxq_s1 {
      h1 {
        font-size: 36px;
        font-weight: bold;
        color: rgba(53, 53, 53, 1);
        line-height: 70px;
      }
      .spxq_s1_1 {
        display: flex;
        p {
          font-size: 22px;
          font-weight: 400;
          color: rgba(236, 81, 78, 1);
          line-height: 36px;
          padding: 5px 14px;
          border-radius: 6px;
          border: 1px solid #F49897;
          margin-right: 16px;
        }
        img {
          width: 18px;
          height: 20px;
          margin-right: 6px;
        }
      }
      .spxq_s1_2 {
        display: flex;
        width: 710px;
        justify-content: space-between;
        border-bottom: 1px solid #E3E3E3;
        margin-top: 24px;
        padding-bottom: 18px;
        p {
          font-size: 24px;
          font-weight: 400;
          color: rgba(118, 118, 118, 1);
          margin-bottom: 10px;
        }
        span {
          font-size: 30px;
          font-weight: bold;
          color: rgba(236, 81, 78, 1);
        }
      }
    }
    .spxq_s2 {
      margin-top: 30px;
      div {
        color: #767676;
        font-size: 24px;
        display: flex;
        margin-top: 14px;
        span {
          color: #353535;
        }
      }
      .spxq_item {
        p {
          width: 330px;
        }
      }
      .spxq_item1 {
        display: flex;
        img {
          width: 16px;
          height: 22px;
          margin-left: 50px;
          margin-right: 6px;
        }
        .spxq_item1_span {
          text-decoration: underline;
          color: #EC514E;
        }
      }
    }
    .spxq_s3 {
      margin-left: -20px;
      img {
        width: 730px;
        height: 264px;
      }
    }
    .spxq_s4 {
      h1 {
        font-size: 34px;
        font-weight: bold;
        color: rgba(26, 26, 26, 1);
        line-height: 42px;
        margin: 10px 0 10px 10px;
      }
    }
    .spxq_bottom {
      width: 750px;
      position: fixed;
      bottom: 0;
      left: 0;
      height: 114px;
      display: flex;
      background: #fff;
      border-top: 1px solid #ddd;
      .spxq_b1 {
        width: 170px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        img {
          width: 40px;
          height: 38px;
        }
        p {
          font-size: 24px;
          font-weight: 500;
          color: rgba(114, 118, 119, 1);
        }
      }
      .spxq_b2 {
        width: 290px;
        height: 114px;
        background: #FEAF01;
        display: flex;
        align-items: center;
        justify-content: center;
        p {
          font-size: 36px;
          font-weight: 500;
          color: rgba(255, 255, 255, 1);
        }
      }
      .spxq_b3 {
        width: 290px;
        height: 114px;
        background: #EC514E;
        display: flex;
        align-items: center;
        justify-content: center;
        p {
          font-size: 36px;
          font-weight: 500;
          color: rgba(255, 255, 255, 1);
        }
      }
    }
  }
</style>
