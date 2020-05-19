<template>
  <div class="service" style="background-image: url('/static/images/找店服务icon/icon-zd-bg@3x.png')">
    <div class="ser_top">
      <div class="ser_top_left">
        <img class="img_1" src="/static/images/找店服务icon/icon-zd-address@3x.png" alt />
        <p>上海</p>
        <img class="img_2" src="/static/images/找店服务icon/icon-zd-bottom@3x.png" alt />
      </div>
      <div class="ser_search">
        <van-search left-icon="/static/images/找店服务icon/icon-zd-search@3x.png" shape="round" placeholder="找店铺 找项目" />
      </div>
    </div>
    <div class="ser_s1" style="background-image: url('/static/images/找店服务icon/icon-zd-xqdj-bg@3x.png')">
      <div class="ser_s1_top">
        <div>
          <img src="/static/images/找店服务icon/icon-zd-xx-btn@3x.png" alt />
          <p>发布信息</p>
          <span>精准匹配</span>
        </div>
        <div>
          <img src="/static/images/找店服务icon/icon-zd-zj-btn@3x.png" alt />
          <p>转店专家</p>
          <span>高效指导</span>
        </div>
        <div>
          <img src="/static/images/找店服务icon/icon-zd-hq-btn@3x.png" alt />
          <p>店铺行情</p>
          <span>一手掌握</span>
        </div>
        <div>
          <img src="/static/images/找店服务icon/icon-zd-fw-btn@3x.png" alt />
          <p>会员服务</p>
          <span>为你定制</span>
        </div>
      </div>
      <div class="ser_s1_btn">
        <img src="/static/images/找店服务icon/icon-zd-xqdj-btn@3x.png" alt />
        <p>找店需求登记</p>
      </div>
    </div>
    <div class="ser_s2" style="background-image: url('/static/images/找店服务icon/icon-zd-tz-bg@3x.png')">
      <div class="ser_s2_1">
        <img src="/static/images/找店服务icon/icon-zd-tz@3x.png" alt="">
        <p>感谢用户133****8888开通转店快服务</p>
      </div>
      <div class="ser_s2_2">
        <span>昨天</span>
        <img src="/static/images/找店服务icon/icon-zd-go@3x.png" alt="" class="ser_s2_go">
      </div>
    </div>
    <div class="ser_s3">
      <div class="ser_s3_1" style="background-image: url('/static/images/找店服务icon/icon-zd-hy-bg@3x.png')">
        <div class="ser_s3_btn" style="background-image: url('/static/images/找店服务icon/icon-zd-btn@3x.png')">
          <p>开通找店会员</p>
        </div>
      </div>
      <div class="ser_s3_2" style="background-image: url('/static/images/找店服务icon/icon-zd-kf-bg@3x.png')">
        <div class="ser_s3_btn2" style="background-image: url('/static/images/找店服务icon/icon-zd-btn@3x.png')">
          <p>立即咨询</p>
        </div>
      </div>
    </div>
    <div class="ser_s4">
      <div class="ser_s4_1">
        <img src="/static/images/找店服务icon/icon-zd-share@3x.png" alt="">
      </div>
      <div class="ser_s4_2">
        <h2>专业顾问为你服务</h2>
        <p>查看更多顾问
          <img src="/static/images/找店服务icon/icon-zd-go@3x.png" alt="">
        </p>
      </div>
      <div class="ser_s4_3">
        <div>
          <img src="/static/images/找店服务icon/icon-zd-pg@3x.png" alt="">
          <p>专业评估 &nbsp;&nbsp;|</p>
        </div>
        <div>
          <img src="/static/images/找店服务icon/icon-zd-tj@3x.png" alt="">
          <p>精准推荐 &nbsp;&nbsp;|</p>
        </div>
        <div>
          <img src="/static/images/找店服务icon/icon-zd-yj@3x.png" alt="">
          <p>撮合议价</p>
        </div>
      </div>
    </div>
    <div class="ser_s5">
      <div v-for="item in 3" :key="item" class="ser_s5_item">
        <div class="ser_s5_top">
          <img class="ser_s5_img" src="/static/images/找店服务icon/tx.jpg" alt="">
          <div>
            <h2>好铺多集团</h2>
            <p>苏贞昌</p>
            <div class="ser_s5_bottom">
              <img src="/static/images/找店服务icon/icon-zd-ljlx-btn@3x.png" alt="">
              <p>立即联系</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {};
</script>

<style lang="scss">
  .service {
    --search-input-height: 34px;
    background-size: 750px 314px;
    background-repeat: no-repeat;
    .ser_top {
      width: 700px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      padding-top: 10px;
      .ser_top_left {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 130px;
        color: #fff;
        .img_1 {
          width: 24px;
          height: 30px;
        }
        .img_2 {
          width: 19px;
          height: 10px;
        }
      }
      .ser_search {
        width: 522px;
        height: 58px;
      }
      .van-search {
        height: 58px;
        padding: 0;
        border-radius: 30px;
        font-size: 20px;
      }
      .van-search__content--round {
        border-radius: 30px;
      }
      .van-search__content {
        height: 58px;
        line-height: 58px;
      }
      .van-cell {
        box-sizing: border-box;
        height: 58px;
        line-height: 58px;
        padding: 6px 10px 5px 4px !important;
      }
    }
    .ser_s1 {
      width: 701px;
      height: 387px;
      margin: 0 auto;
      background-size: 701px 387px;
      margin-top: 112px;
      .ser_s1_top {
        width: 564px;
        height: 162px;
        padding-top: 56px;
        padding-left: 72px;
        display: flex;
        justify-content: space-between;
        div {
          display: flex;
          flex-direction: column;
          justify-content: space-between;
          align-items: center;
          img {
            width: 88px;
            height: 88px;
          }
          p {
            color: #333333;
            font-size: 24px;
            margin-bottom: -4px;
          }
          span {
            color: #666666;
            font-size: 18px;
          }
        }
      }
      .ser_s1_btn {
        margin-top: 40px;
        text-align: center;
        position: relative;
        img {
          width: 462px;
          height: 75px;
        }
        p {
          font-size: 30px;
          color: #fff;
          position: absolute;
          top: 14px;
          left: 254px;
        }
      }
    }
    .ser_s2 {
      width: 677px;
      height: 49px;
      background-size: 677px 49px;
      background-repeat: no-repeat;
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin: 0 auto;
      padding: 4px 20px;
      margin-top: 20px;
      box-sizing: border-box;
      .ser_s2_1 {
        color: #333333;
        font-size: 18px;
        display: flex;
        img {
          width: 23px;
          height: 22px;
          margin-right: 20px;
        }
      }
      .ser_s2_2 {
        color: #6C6C6C;
        font-size: 18px;
        display: flex;
        line-height: 18px;
        img {
          margin-left: 17px;
          width: 9px;
          height: 16px;
        }
      }
    }
    .ser_s3 {
      width: 670px;
      margin: 0 auto;
      margin-top: 39px;
      .ser_s3_1 {
        position: relative;
        background-size: 670px 292px;
        background-repeat: no-repeat;
        height: 292px;
      }
      .ser_s3_2 {
        position: relative;
        background-size: 670px 99px;
        background-repeat: no-repeat;
        height: 99px;
        margin-top: 29px;
      }
      .ser_s3_btn {
        position: absolute;
        right: 56px;
        bottom: 36px;
        width: 177px;
        height: 48px;
        background-size: 177px 48px;
        background-repeat: no-repeat;
        p {
          color: #EC514E;
          font-size: 24px;
          text-align: center;
          line-height: 48px;
        }
      }
      .ser_s3_btn2 {
        position: absolute;
        right: 56px;
        bottom: 24px;
        width: 177px;
        height: 48px;
        background-size: 177px 48px;
        background-repeat: no-repeat;
        p {
          color: #EC514E;
          font-size: 24px;
          text-align: center;
          line-height: 48px;
        }
      }
    }
    .ser_s4 {
      width: 670px;
      display: flex;
      flex-direction: column;
      margin: 0 auto;
      margin-top: 60px;
      .ser_s4_1 {
        img {
          width: 364px;
          height: 45px;
        }
      }
      .ser_s4_2 {
        display: flex;
        justify-content: space-between;
        margin-top: 29px;
        h2 {
          color: #333333;
          font-size: 32px;
          font-weight: bold;
        }
        p {
          color: #6C6C6C;
          font-size: 18px;
          line-height: 46px;
        }
        img {
          width: 9px;
          height: 16px;
          margin-left: 18px;
        }
      }
      .ser_s4_3 {
        display: flex;
        margin-top: 20px;
        div {
          display: flex;
          font-size: 20px;
          line-height: 20px;
          color: #ACACAC;
          margin-right: 14px;
        }
        img {
          width: 22px;
          height: 22px;
          margin-right: 10px;
        }
      }
    }
    .ser_s5 {
      width: 730px;
      height: 168px;
      display: flex;
      justify-content: space-between;
      margin: 0 auto;
      margin-top: 36px;
      margin-bottom: 74px;
      .ser_s5_item {
        width: 222px;
        height: 166px;
        border-radius: 10px;
        box-shadow: 0px 2px 4px 0px rgba(6, 0, 1, 0.4);
        .ser_s5_top {
          display: flex;
          margin-top: 20px;
          .ser_s5_img {
            width: 70px;
            height: 70px;
            border-radius: 50%;
            margin-right: 12px;
            margin-left: 4px;
          }
          h2 {
            font-size: 24px;
            color: #1F1E1E;
            margin-top: 10px;
            font-weight: bold;
          }
          p {
            font-size: 14px;
            color: #1F1E1E;
            margin-top: 6px;
          }
          .ser_s5_bottom {
            width: 100px;
            height: 41px;
            margin-top: 20px;
            position: relative;
            img {
              width: 100px;
              height: 41px;
            }
            p {
              position: absolute;
              top: 0;
              left: 10px;
              font-size: 20px;
              color: #fff;
            }
          }
        }
      }
    }
  }
</style>
