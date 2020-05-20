<template>
  <div class="pd">
    <div class="pd_top">
      <h2>
        <p></p>
        拍店攻略
      </h2>
      <h3>
        <img src="http://wynode.com/haopuduo/拍店服务icon/icon-pdfw-pdjl@3x.png" alt="">
        <span>拍店记录</span>
      </h3>
    </div>
    <div class="pd_s1">
      <h2>
        <img src="http://wynode.com/haopuduo/拍店服务icon/icon-pdfw-bt@3x.png" alt="">
        <span>定位坐标</span>
      </h2>
      <h3>
        <span>未定位</span>
        <img src="http://wynode.com/haopuduo/拍店服务icon/icon-pdfw-go@3x.png" alt="">
      </h3>
    </div>
    <div class="pd_s2">
      <img src="http://wynode.com/haopuduo/拍店服务icon/icon-pdfw-bt@3x.png" alt="">
      <p>店主电话： </p>
      <span> 请输入手机号</span>
    </div>
    <div class="pd_center">
      <h2>
        上传图片
      </h2>
      <div class="pd_s3">
        <div>
          <img src="http://wynode.com/haopuduo/拍店服务icon/icon-pdfw-sczp@3x.png" alt="">
          <p>商铺正面照</p>
        </div>
        <div>
          <img src="http://wynode.com/haopuduo/拍店服务icon/icon-pdfw-sczp@3x.png" alt="">
          <p>商铺左侧照</p>
        </div>
      </div>
      <div class="pd_s4">
        <div>
          <img src="http://wynode.com/haopuduo/拍店服务icon/icon-pdfw-sczp@3x.png" alt="">
          <p>商铺右侧照</p>
        </div>
        <div>
          <img src="http://wynode.com/haopuduo/拍店服务icon/icon-pdfw-sczp@3x.png" alt="">
          <p>电话张贴图</p>
        </div>
      </div>
      <div class="pd_s5">
        <div>
          <img src="http://wynode.com/haopuduo/拍店服务icon/icon-pdfw-sczp@3x.png" alt="">
          <p>上传视频（15-60s）</p>
        </div>
      </div>
    </div>
    <div class="pd_s6">
      <h2>温馨提示：</h2>
      <p>1、请在白天光线好时拍摄，注意招牌不要有反光；</p>
      <p>2、请务必横向拍摄；</p>
      <p>3、尽量拍摄完整的店铺照片，照片中不要有行人和车辆等；</p>
      <p>4、请站在店铺前进行定位，务必定位出店铺的准确坐标，不准确会降低审核通过率</p>
      <p>5、店面内景照片务必上传</p>
    </div>
    <div class="pd_s7">
      <img src="http://wynode.com/haopuduo/拍店服务icon/icon-pdfw-btn@3x.png" alt="">
      <h2>发布</h2>
    </div>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss">
  .pd {
    width: 690px;
    margin: 0 auto;
    margin-top: 20px;
    .pd_top {
      display: flex;
      justify-content: space-between;
      align-items: center;
      h2 {
        display: flex;
        font-size: 30px;
        font-weight: bold;
        color: #616161;
        p {
          width: 8px;
          height: 30px;
          background: #616161;
          border-radius: 4px;
          margin-right: 14px;
        }
      }
      h3 {
        color: #616161;
        font-size: 20px;
        img {
          width: 21px;
          height: 24px;
          margin-right: 8px;
        }
      }
    }
    .pd_s1 {
      background: #F3F3F5;
      border-radius: 36px;
      margin-top: 36px;
      height: 64px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      h2 {
        img {
          width: 20px;
          height: 20px;
          margin-left: 28px;
          margin-right: 14px;
        }
        span {
          color: #616161;
          font-size: 28px;
        }
      }
      h3 {
        color: #616161;
        font-size: 24px;
        img {
          width: 10px;
          height: 20px;
          margin-left: 14px;
          margin-right: 40px;
        }
      }
    }
    .pd_s2 {
      display: flex;
      align-items: center;
      background: #F3F3F5;
      border-radius: 36px;
      height: 64px;
      margin-top: 26px;
      img {
        width: 20px;
        height: 20px;
        margin-left: 28px;
        margin-right: 14px;
      }
      p {
        color: #616161;
        font-size: 28px;
      }
      span {
        color: #616161;
        font-size: 22px;
      }
    }
    .pd_center {
      width: 640px;
      margin: 0 auto;
      h2 {
        font-size: 30px;
        font-weight: bold;
        margin-top: 40px;
        color: rgba(97, 97, 97, 1);
      }
    }
    .pd_s3 {
      margin-top: 24px;
      display: flex;
      justify-content: space-between;
      div {
        width: 282px;
        height: 218px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border-radius: 8px;
        border: 1px solid #DDDDDD;
        img {
          width: 94px;
          height: 94px;
          margin-bottom: 20px;
        }
        p {
          font-size: 30px;
          font-weight: 400;
          color: rgba(219, 219, 219, 1);
        }
      }
    }
    .pd_s4 {
      margin-top: 28px;
      display: flex;
      justify-content: space-between;
      div {
        width: 282px;
        height: 218px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border-radius: 8px;
        border: 1px solid #DDDDDD;
        img {
          width: 94px;
          height: 94px;
          margin-bottom: 20px;
        }
        p {
          font-size: 30px;
          font-weight: 400;
          color: rgba(219, 219, 219, 1);
        }
      }
    }
    .pd_s5 {
      margin-top: 28px;
      div {
        width: 640px;
        height: 218px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border-radius: 8px;
        border: 1px solid #DDDDDD;
      }
      img {
        width: 94px;
        height: 94px;
        margin-bottom: 20px;
      }
      p {
        font-size: 30px;
        font-weight: 400;
        color: rgba(219, 219, 219, 1);
      }
    }
    .pd_s6 {
      margin-top: 30px;
      h2 {
        font-size: 24px;
        font-weight: 400;
        color: rgba(236, 81, 78, 1);
        line-height: 17px;
        margin-bottom: 24px;
      }
      p {
        margin-left: 30px;
        font-size: 20px;
        font-weight: 400;
        color: rgba(150, 150, 150, 1);
        line-height: 32px;
      }
    }
    .pd_s7 {
      position: relative;
      width: 640px;
      margin: 0 auto;
      margin-top: 30px;
      margin-bottom: 30px;
      img {
        width: 630px;
        height: 88px;
        margin: 0 auto;
      }
      h2 {
        font-size: 36px;
        font-weight: 600;
        color: rgba(255, 255, 255, 1);
        position: absolute;
        top: 20px;
        left: 286px;
      }
    }
  }
</style>
