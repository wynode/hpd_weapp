<template>
  <div class="c_section2">
    <div class="c_section2_left">
      <image :src="imgUrl" class="c_section2_left_img"></image>
    </div>

    <div class="c_section2_right">
      <div class="csr2_top">厦门市思明区望海路软件园二期朝</div>
      <div class="csr2_top_2">望海路-软件园二期 | 200㎡</div>
      <div class="csr2_center" v-if="btntype == 'warning'">
        <van-button round plain type="warning" size="mini" color="#EC514E" class="csr2_btn">餐饮美食</van-button>
        <van-button round plain type="warning" size="mini" color="#EC514E" class="csr2_btn">奶茶糕点</van-button>
        <van-button round plain type="warning" size="mini" color="#EC514E" class="csr2_btn">生鲜水果</van-button>
        <van-button round plain type="warning" size="mini" color="#EC514E" class="csr2_bt">其他</van-button>
      </div>
      <div class="csr2_center" v-else>
        <van-button round plain type="default" size="mini" color="#A7A7A7" class="csr2_btn">餐饮美食</van-button>
        <van-button round plain type="default" size="mini" color="#A7A7A7" class="csr2_btn">奶茶糕点</van-button>
        <van-button round plain type="default" size="mini" color="#A7A7A7" class="csr2_btn">生鲜水果</van-button>
        <van-button round plain type="default" size="mini" color="#A7A7A7" class="csr2_bt">其他</van-button>
      </div>
      <div class="csr2_bottom">
        <div>￥18800元<span> /月</span></div>
        <p>05-09 08:55</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imgUrl: {
      type: String,
      default: "http://wynode.com/haopuduo/首页icon/room.jpg",
    },
    btntype: {
      type: String,
      default: "warning",
    }
  },
};
</script>

<style>
.c_section2 {
  width: 690px;
  padding: 14px 0;
  margin: 0 auto;
  display: flex;
}

.c_section2_left_img {
  width: 270px;
  height: 164px;
  border-radius: 8px;
}

.c_section2_right {
  overflow: hidden;
  margin-left: 16px;
  width: 416px;
}
.csr2_top {
  color: #434343;
  font-size: 26px;
  margin-top: 4px;
  white-space: nowrap;
  overflow: hidden;
}
.csr2_top_2 {
  color: #7a7a7a;
  font-size: 24px;
  margin-top: 8px;
}
.csr2_center {
  display: flex;
  justify-content: space-between;
  margin-top: 8px;
}
.csr2_btn .van-button {
  width: 106px;
  height: 32px;
  margin-right: 8px;
  font-size: 22px;
  line-height: 30px;
  border-radius: 10px;
}
.csr2_bt .van-button {
  min-width: 20px;
  width: 58px;
  height: 32px;
  font-size: 22px;
  line-height: 30px;
  border-radius: 10px;
}

.csr2_bottom {
  display: flex;
  justify-content: space-between;
  margin-top: 8px;
  color: #ec514e;
  font-size: 28px;
  font-weight: bold;
}
.csr2_bottom span {
  color: #ec514e;
  font-size: 26px;
}
.csr2_bottom p {
  color: #7A7A7A;
  font-size: 18px;
  font-weight: 400;
  align-self: center;
  margin-top: 8px;
}


</style>
