<template>
  <div class="c_title">
    <div class="ct_left">
      <div class="ct_before"></div>
      <div class="ct_title">{{ title }}</div>
    </div>
    <div class="ct_right" v-if="showMore" @click="gopuyuan">
      <div class="ct_right_more">
        <p>查看更多</p>
        <img src="http://wynode.com/haopuduo/首页icon/icon-sy-go@3x.png" alt="" class="ct_image">
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    props: {
      title: {
        type: String,
        default: '标题'
      },
      showMore: {
        type: Boolean,
        default: true,
      }
    },
    methods: {
      gopuyuan() {
        const url = "/pages/puyuan/main";
        wx.switchTab({ url })
      },
    },
  };
</script>

<style>
  .c_title {
    width: 670px;
    height: 48px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
  }
  .ct_left {
    width: 500px;
    display: flex;
    align-items: center;
  }
  .ct_before {
    width: 4px;
    height: 25px;
    background: #EC514E;
  }
  .ct_title {
    font-size: 30px;
    color: #1A1A1A;
    margin-left: 14px;
  }
  .ct_right {
    color: #858585;
    font-size: 20px;
    line-height: 1;
    display: flex;
    align-items: flex-end;
  }
  .ct_right_more {
    height: 20px;
    display: flex;
  }
  .ct_image {
    width: 9px;
    height: 16px;
    margin-top: 2px;
    margin-left: 9px;
  }
</style>


