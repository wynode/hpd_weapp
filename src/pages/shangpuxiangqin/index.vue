<template>
  <div class="spxq">
    <div class="spxq_top">
      <img src="/static/images/商铺详情icon/bg1.jpg" alt="">
    </div>
    <div class="spxq_s1">
      <h1>望海路软件园二期公寓低价转让</h1>
      <div class="spxq_s1_1">
        <p><img src="/static/images/商铺详情icon/icon-shop-hot@3x.png" alt="">热门</p>
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
          <span>60</span>
        </div>
        <div>
          <p>转让费（万元/月）/月）</p>
          <span>60</span>
        </div>
      </div>
    </div>
    <div class="spxq_s2">
      <div>
        <p>区域：<span>鼓楼区-西洪路</span></p>
        <p>商圈：<span>金牛山</span></p>
      </div>
      <div>
        <p>小区：<span>万隆花园一期</span></p>
        <p>面宽：<span>4米</span></p>
      </div>
      <div>
        <p>进深：<span>4米</span></p>
        <p>层高：<span>4米</span></p>
      </div>
      <div>
        <p>地址：<span>鼓楼区西洪路457-2美华隆佳便利</span></p>
        <img src="/static/images/商铺详情icon/ckdt.jpg" alt="">
      </div>
      <div>
        <p>地址：<span>望海路软件园二期公寓靠近地铁商超，周边交通便利，生活环境优越...</span></p>
      </div>
    </div>
    <div class="spxq_s3">
      <img src="/static/images/商铺详情icon/icon-shop-ad@3x.png" alt="">
    </div>
    <div class="spxq_s4">
      <h1>
        猜你喜欢
      </h1>
      <secitem v-for="item in 10" :key="item"></secitem>
    </div>
    <div class="spxq_bottom">
      <div class="spxq_b1">
        <img src="/static/images/商铺详情icon/icon-shop-wsc@3x.png" alt="" @click="showRed = true" v-if="!showRed">
        <img src="/static/images/商铺详情icon/icon-shop-ysc@3x.png" alt="" @click="showRed = false" v-else>
        <p>收藏</p>
      </div>
      <div class="spxq_b1">
        <p>已租提醒</p>
      </div>
      <div class="spxq_b1">
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
      img {
        width: 710px;
        height: 316px;
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
        p {
          font-size: 22px;
          font-weight: 400;
          color: rgba(236, 81, 78, 1);
          line-height: 36px;
          padding: 5px 14px;
          border-radius: 6px;
        }
        img {
          width: 18px;
          height: 20px;
        }
      }
      .spxq_s1_2 {
        display: flex;
        width: 710px;
        justify-content: space-between;
        border-bottom: 1px solid #E3E3E3;
        p {
          font-size: 24px;
          font-weight: 400;
          color: rgba(118, 118, 118, 1);
        }
        span {
          font-size: 30px;
          font-weight: bold;
          color: rgba(236, 81, 78, 1);
        }
      }
    }
    .spxq_s2 {
      div {
        color: #767676;
        font-size: 24px;
        display: flex;
        span {
          color: #353535;
        }
      }
    }
    .spxq_s3 {
      img {
        width: 710px;
        height: 264px;
      }
    }
    .spxq_s4 {
      h1 {
        font-size: 34px;
        color: #1A1A1A;
      }
    }
    .spxq_bottom {
      width: 750px;
      position: fixed;
      height: 114px;
      display: flex;
      border-top: 1px solid #ddd;
      .spxq_b1 {
        width: 170px;
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
        p {
          font-size: 36px;
          font-weight: 500;
          color: rgba(255, 255, 255, 1);
          display: flex;
          align-items: center;
          justify-content: center;
        }
      }
      .spxq_b3 {
        width: 290px;
        height: 114px;
        background: #EC514E;
        p {
          font-size: 36px;
          font-weight: 500;
          color: rgba(255, 255, 255, 1);
          display: flex;
          align-items: center;
          justify-content: center;
        }
      }
    }
  }
</style>
