<template>
  <div class="c_card">
    <div class="c_card_top">
      <image :src="imgUrl" class="c_card_top_img"></image>
      <div class="c_card_top_tag" v-if="tagContent">
        {{ tagContent }}
      </div>
    </div>

    <div class="c_card_bottom">
      <div class="ccb_top">
        丰台-科技园区 | 140㎡
      </div>
      <div class="ccb_bottom">
        可餐饮 可明火 宽门面 临近学校
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    tagContent: {
      type: String,
      default: '',
    },
    imgUrl: {
      type: String,
      default: '/static/images/首页icon/card1.jpg'
    }
  },
}
</script>

<style>
.c_card {
  width: 100%;
  border-radius: 8px;
  overflow: hidden;
  box-shadow:0px 4px 8px 0px rgba(210, 210, 210, 0.35);
  height: 300px;
}
.c_card_top {
  width: 100%;
  height: 218px;
  position: relative;
}
.c_card_top_img {
  width: 100%;
  height: 218px;
}
.c_card_top_tag {
  position: absolute;
  bottom: 18px;
  right: 18px;
  padding: 8px 6px;
  font-size: 14px;
  color: #858585;
  background: #fff;
  border-radius: 4px;
}
.c_card_bottom {
  overflow: hidden;
  padding: 12px 10px;
}
.ccb_top {
  font-size: 18px;
  color: #131313;
}
.ccb_bottom {
  margin-top: 10px;
  font-size: 16px;
  color: #6E6E6E;
  white-space: nowrap;
  overflow: hidden;
}
</style>
