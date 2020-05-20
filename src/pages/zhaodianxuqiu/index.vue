<template>
  <div class="zdxq">
    <div class="zdxq_top">
      <van-cell-group>
        <van-field label="行业" is-link placeholder="请选择" placeholder-style="text-align: right" />
        <van-field label="面积" placeholder="最小  最大  平米" placeholder-style="text-align: right" />
        <van-field label="期望租金" placeholder-style="text-align: right">
          <div slot="button" class="zdxq_btn">
            <img src="http://wynode.com/haopuduo/找店需求icon/icon-zd-xz@3x.png" alt="">
            <div>
              <span>面议</span>
              <span style="color: #EC514E">填写</span>
            </div>
          </div>
        </van-field>
        <van-field label="区域" is-link placeholder="请选择" placeholder-style="text-align: right" />
        <van-field label="要求" is-link placeholder="请填写具体的找点要求" placeholder-style="text-align: right" />
        <van-field label="联系人" placeholder="请填写" placeholder-style="text-align: right" />
        <van-field value="88888888" label="手机号码" placeholder="" placeholder-style="text-align: right" />
      </van-cell-group>
    </div>
    <div class="zdxq_s1">
      <p>填写越详细匹配越精细哦~</p>
      <div>
        <img src="http://wynode.com/haopuduo/找店需求icon/icon-zd-btn@3x.png" alt="">
        <h2>发布</h2>
      </div>
    </div>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss">
  .zdxq {
    .van-field__input {
      text-align: right;
    }
    .van-hairline--top-bottom {
      &::after {
        border: 0;
      }

    }
    .zdxq_btn {
      width: 124px;
      height: 32px;
      position: relative;
      img {
        width: 124px;
        height: 34px;
      }
      div {
        position: absolute;
        top: -10px;
        left: 0;
      }
      span {
        color: #fff;
        font-size: 20px;
        line-height: 32px;
        margin-left: 14px;
      }
    }
    .zdxq_s1 {
      text-align: center;
      p {
        font-size: 18px;
        font-weight: 400;
        color: rgba(219, 219, 219, 1);
        margin-top: 100px;
        margin-bottom: 56px;
      }
      div {
        position: relative;
        width: 690px;
        margin: 0 auto;
      }
      img {
        width: 690px;
        height: 88px;
        margin: 0 auto;
      }
      h2 {
        font-size: 36px;
        font-weight: 600;
        color: rgba(255, 255, 255, 1);
        position: absolute;
        top: 20px;
        left: 300px;
      }
    }
    .zdxq_top {
      margin-top: 20px;
    }
  }
</style>
