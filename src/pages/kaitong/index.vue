<template>
  <div class="kt">
    <div class="kt_top">
      <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-bg@3x.png" alt="">
      <div class="kt_top_info">
        <img src="http://wynode.com/haopuduo/开通找店会员icon/tx.jpg" alt="">
        <div>
          <p>用户ID：13311118888</p>
          <span>您还不是会员哦~</span>
        </div>
      </div>
    </div>
    <div class="kt_s1">
      <h1>会员特权</h1>
      <div class="kt_s1_ul">
        <div class="kt_s1_item">
          <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-mfck@3x.png" alt="">
          <p>免费查看</p>
        </div>
        <div class="kt_s1_item">
          <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-mffb@3x.png" alt="">
          <p>免费发布</p>
        </div>
        <div class="kt_s1_item">
          <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-msyj@3x.png" alt="">
          <p>免收佣金</p>
        </div>
        <div class="kt_s1_item">
          <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-ztfd@3x.png" alt="">
          <p>直通房东</p>
        </div>
      </div>
    </div>
    <div class="kt_s2" style="background-image: url('http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-ljzx-bg@3x.png')">
      <div class="kt_s2_left">
        <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-vip@3x.png" alt="">
        <p>更多升级服务请点击咨询</p>
      </div>
      <div class="kt_s2_right">
        <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-ljzx-rectangle@3x.png" alt="">
        <p>立即咨询</p>
      </div>
    </div>
    <div class="kt_s3">
      <h1>开通会员</h1>
      <div class="kt_s3_content">
        <div class="kt_s3_1">
          <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-kthy-bg1@3x.png" alt="">
          <div class="kt_s3_item">
            <p>10天</p>
            <p>￥<span>9.8</span></p>
            <p style="opacity:0.5;">原价:￥<em style="text-decoration:underline">39</em></p>
            <h3 style="opacity:0.7;">(仅享受一次)</h3>
          </div>
        </div>
        <div class="kt_s3_2">
          <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-kthy-bg2@3x.png" alt="">
          <div class="kt_s3_item">
            <p>30天</p>
            <p>￥<span>68</span></p>
            <p style="opacity:0.5;">原价:￥<em style="text-decoration:underline">118</em></p>
            <h3 style="opacity:0.7;">(仅享受一次)</h3>
          </div>
        </div>
        <div class="kt_s3_3">
          <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-kthy-bg3@3x.png" alt="">
          <div class="kt_s3_item">
            <p>30天</p>
            <p>￥<span>68</span></p>
            <p style="opacity:0.5;">原价:￥<em style="text-decoration:underline">118</em></p>
          </div>
        </div>
      </div>
    </div>
    <div class="kt_s4">
      <div class="kt_s4_1">
        <img src="http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-choose@3x.png" alt="">
        <p>购买即视为同意<span style="color: #EC514E">《会员服务协议》</span></p>
      </div>
      <div style="background-image: url('http://wynode.com/haopuduo/开通找店会员icon/icon-zdhy-btn@3x.png')" class="kt_s4_2">
        <p>立即开通</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss" scoped>
  .kt {
    width: 670px;
    margin: 0 auto;
    .kt_top {
      margin-top: 10px;
      position: relative;
      img {
        width: 670px;
        height: 386px;
      }
      .kt_top_info {
        display: flex;
        position: absolute;
        top: 50px;
        left: 40px;
        img {
          width: 104px;
          height: 104px;
          border-radius: 50%;
        }
        div {
          margin-left: 18px;
        }
        p {
          color: #fff;
          font-size: 24px;
          margin-top: 22px;
        }
        span {
          color: #fff;
          font-size: 18px;
          opacity: 0.7;
          margin-top: 16px;
        }
      }
    }
    .kt_s1 {
      h1 {
        color: #1A1A1A;
        font-size: 30px;
        font-weight: bold;
      }
      .kt_s1_ul {
        display: flex;
        justify-content: space-between;
        margin-top: 26px;
      }
      .kt_s1_item {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        img {
          width: 97px;
          height: 97px;
        }
        p {
          color: #333;
          font-size: 22px;
          margin-top: 14px;
        }
      }
    }
    .kt_s2 {
      position: relative;
      height: 82px;
      display: flex;
      background-size: 670px 82px;
      background-repeat: no-repeat;
      align-items: center;
      justify-content: space-between;
      margin-top: 36px;
      .kt_s2_left {
        display: flex;
        align-items: center;
        margin-left: 22px;
        img {
          width: 24px;
          height: 24px;
          margin-right: 24px;
        }
        p {
          font-size: 28px;
          color: #EC514E;
          font-weight: 500;
        }
      }
      .kt_s2_right {
        position: relative;
        margin-right: 20px;
        img {
          width: 128px;
          height: 44px;
        }
        p {
          color: #EC514E;
          font-size: 22px;
          position: absolute;
          top: 6px;
          left: 20px;
        }
      }
    }
    .kt_s3 {
      margin-top: 40px;
      h1 {
        font-size: 30px;
        font-weight: bold;
        color: #1A1A1A;
      }
      .kt_s3_content {
        display: flex;
        justify-content: space-between;
        height: 254px;
        align-items: flex-end;
        position: relative;
        text-align: center;
        margin-top: 32px;
        p {
          color: #333;
          font-size: 26px;
          display: flex;
          align-items: flex-end;
        }
        h3 {
          font-size: 18px;
          font-weight: bold;
          color: rgba(191, 191, 191, 1);
          margin-top: 10px;
        }
        .kt_s3_item {
          width: 200px;
          text-align: center;
          position: absolute;
          top: 30px;
          left: 0;
          display: flex;
          flex-direction: column;
          align-items: center;
          span {
            font-size: 50px;
            line-height: 0.9;
          }
          p {
            margin-top: 10px;
          }
        }
        .kt_s3_1 {
          position: relative;
          img {
            width: 200px;
            height: 236px;
          }
          p {
            color: #FF4676;
            font-size: 26px;
            span {
              font-size: 50px;
            }
            em {
              text-decoration: underline;
            }
          }
        }
        .kt_s3_2 {
          position: relative;
          .kt_s3_item {
            top: 46px;
          }
          img {
            width: 200px;
            height: 253px;
          }
        }
        .kt_s3_3 {
          position: relative;
          img {
            width: 200px;
            height: 236px;
          }
        }
      }
    }
    .kt_s4 {
        margin-top: 52px;
      .kt_s4_1 {
        display: flex;
        align-items: center;
        margin-left: 16px;
        img {
          width: 23px;
          height: 23px;
          margin-right: 10px;
        }
        p {
          color: #999;
          font-size: 22px;
        }
      }
      .kt_s4_2 {
        background-size:670px 85px;
        width: 670px;
        height: 85px;
        display: flex;
        justify-content: center;
        align-items: center;
        color: #fff;
        font-size: 30px;
        margin-top: 14px;
        margin-bottom: 60px;
      }
    }
  }
</style>
