<template>
  <div class="c_section">
    <div class="c_section_left">
      <image :src="imgUrl" class="c_section_left_img"></image>
    </div>

    <div class="c_section_right">
      <div class="csr_top">思明区-软件园二期 | 200㎡</div>
      <div class="csr_center">望海路-软件园二期 <p class="csr_center_p">￥1.8万<span> /月</span></p></div>
      <div class="csr_bottom">
        <van-button round plain type="warning" size="mini" color="#EC514E">餐饮美食</van-button>
        <van-button round plain type="info" size="mini">奶茶糕点</van-button>
        <van-button round plain type="primary" size="mini">生鲜水果</van-button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imgUrl: {
      type: String,
      default: 'http://wynode.com/haopuduo/首页icon/section.jpg'
    }
  },
}
</script>

<style>
.c_section {
  width: 670px;
  height: 146px;
  margin: 0 auto;
  display: flex;
}

.c_section_left_img {
  width: 222px;
  height: 146px;
  border-radius: 6px;
}

.c_section_right {
  overflow: hidden;
  margin-left: 10px;
  width: 428px;
}
.csr_top {
  color: #434343;
  font-size: 28px;
  margin-top: 10px;
}
.csr_center {
  color: #7A7A7A;
  font-size: 24px;
  margin-top: 10px;
  display: flex;
  justify-content: space-between;
}
.csr_center .csr_center_p{
  color: #EC514E;
  font-size: 28px;
  font-weight: bold;
}
.csr_center span{
  color: #EC514E;
  font-size: 26px;
}
.csr_bottom {
  display: flex;
  margin-top: 10px;
}
.csr_bottom .van-button {
  width: 102px;
  height: 30px;
  margin-right: 8px;
  font-size: 20px;
  line-height: 26px;
}
</style>
