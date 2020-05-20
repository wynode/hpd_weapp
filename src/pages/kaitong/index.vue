<template>
  <div class="kt">
    <div class="kt_top">
      <img src="/static/images/开通找店会员icon/icon-zdhy-bg@3x.png" alt="">
      <div class="kt_top_info">
        <img src="/static/images/开通找店会员icon/tx.jpg" alt="">
        <div>
          <p>用户ID：13311118888</p>
          <span>您还不是会员哦~</span>
        </div>
      </div>
    </div>
    <div class="kt_s1">
      <h1>会员特权</h1>
      <div class="kt_s1_item">
        <img src="/static/images/开通找店会员icon/icon-zdhy-mfck@3x.png" alt="">
        <p>免费查看</p>
      </div>
      <div class="kt_s1_item">
        <img src="/static/images/开通找店会员icon/icon-zdhy-mffb@3x.png" alt="">
        <p>免费发布</p>
      </div>
      <div class="kt_s1_item">
        <img src="/static/images/开通找店会员icon/icon-zdhy-msyj@3x.png" alt="">
        <p>免收佣金</p>
      </div>
      <div class="kt_s1_item">
        <img src="/static/images/开通找店会员icon/icon-zdhy-ztfd@3x.png" alt="">
        <p>直通房东</p>
      </div>
    </div>
    <div class="kt_s2" style="background-image: url('/static/images/开通找店会员icon/icon-zdhy-ljzx-bg@3x.png')">
      <div class="kt_s2_left">
        <img src="/static/images/开通找店会员icon/icon-zdhy-vip@3x.png" alt="">
        <p>更多升级服务请点击咨询</p>
      </div>
      <div class="kt_s2_right">
        <img src="/static/images/开通找店会员icon/icon-zdhy-ljzx-rectangle@3x.png" alt="">
        <p>立即咨询</p>
      </div>
    </div>
    <div class="kt_s3">
      <h1>开通会员</h1>
      <div class="kt_s3_content">
        <div class="kt_s3_1">
          <img src="/static/images/开通找店会员icon/icon-zdhy-kthy-bg1@3x.png" alt="">
          <div>
            <p>10天</p>
            <p>￥<span>9.8</span></p>
            <p style="opacity:0.5;">原价:￥<em style="text-decoration:underline">39</em></p>
            <p style="opacity:0.5;">(仅享受一次)</p>
          </div>
        </div>
        <div class="kt_s3_2">
          <img src="/static/images/开通找店会员icon/icon-zdhy-kthy-bg2@3x.png" alt="">
          <div>
            <p>30天</p>
            <p>￥<span>68</span></p>
            <p opacity:0.5;>原价:￥<em style="text-decoration:underline">118</em></p>
            <p opacity:0.5;>(仅享受一次)</p>
          </div>
        </div>
        <div class="kt_s3_3">
          <img src="/static/images/开通找店会员icon/icon-zdhy-kthy-bg3@3x.png" alt="">
          <div>
            <p>30天</p>
            <p>￥<span>68</span></p>
            <p opacity:0.5;>原价:￥<em style="text-decoration:underline">118</em></p>
          </div>
        </div>
      </div>
    </div>
    <div class="kt_s4">
      <div class="kt_s4_1">
        <img src="/static/images/开通找店会员icon/icon-zdhy-choose@3x.png" alt="">
        <p>开通即视为同意<span style="color: #EC514E">《会员服务协议》</span></p>
      </div>
      <div style="background-image: url('/static/images/开通找店会员icon/icon-zdhy-btn@3x.png')" class="kt_s4_2">
        <p>立即开通</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
  }
</script>

<style lang="scss" scoped>
  .kt {
    width: 670px;
    margin: 0 auto;
    .kt_top {
      img {
        width: 670px;
        height: 386px;
      }
      .kt_top_info {
        display: flex;
        img {
          width: 104px;
          height: 104px;
        }
        p {
          color: #fff;
          font-size: 24px;
        }
        span {
          color: #fff;
          font-size: 18px;
        }
      }
    }
    .kt_s1 {
      h1 {
        color: #1A1A1A;
        font-size: 30px;
        font-weight: bold;
      }
      .kt_s1_item {
        img {
          width: 97px;
          height: 97px;
        }
        p {
          color: #333;
          font-size: 22px;
        }
      }
    }
    .kt_s2 {
      position: relative;
      height: 82px;
      display: flex;
      background-size: 670px 82px;
      background-repeat: no-repeat;
      .kt_s2_left {
        display: flex;
        img {
          width: 24px;
          height: 24px;
          margin-right: 28px;
        }
        p {
          font-size: 28px;
          color: #EC514E;
          font-weight: 500;
        }
      }
      .kt_s2_right {
        position: relative;
        img {
          width: 128px;
          height: 44px;
        }
        p {
          color: #EC514E;
          font-size: 22px;
          position: absolute;
          top: 10px;
          left: 20px;
        }
      }
    }
    .kt_s3 {
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
        p {
          color: #333;
          font-size: 26px;
        }
        .kt_s3_1 {
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
          img {
            width: 200px;
            height: 253px;
          }
        }
        .kt_s3_3 {
          img {
            width: 200px;
            height: 236px;
          }
        }
      }
    }
    .kt_s4 {
      .kt_s4_1 {
        display: flex;
        p {
          color: #999;
          font-size: 22px;
        }
      }
      .kt_s4_2 {
        width: 670px;
        height: 85px;
        display: flex;
        justify-content: center;
        align-items: center;
        color: #fff;
        font-size: 30px;
        margin-top: 14px;
      }
    }
  }
</style>
