<template>
  <div class="hezuo">
    <div v-for="item in 10" :key="item" class="hezuo_item">
      <div class="hezuo_left">
        <img class="hezuo_img1" src="http://wynode.com/haopuduo/品牌合作icon/icon-pphz-bg@3x.png" alt="">
        <img class="hezuo_img2" src="http://wynode.com/haopuduo/品牌合作icon/heytea.png" alt="">
      </div>
      <div class="hezuo_right">
        <h1>喜茶</h1>
        <p>面积范围：<span>300-600㎡</span></p>
        <p>计划开店：<span>10家</span></p>
        <p>租金预算：<span>40.0元/天/㎡</span></p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss">
  .hezuo {
    width: 630px;
    height: 192px;
    padding-top: 20px;
    margin: 0 auto;
    .hezuo_item {
      display: flex;
      margin-top: 12px;
      justify-content: space-between;
      .hezuo_left {
        position: relative;
        .hezuo_img1 {
          width: 185px;
          height: 185px;
        }
        .hezuo_img2 {
          width: 140px;
          height: 140px;
          position: absolute;
          top: 22px;
          left: 22px;
        }
      }
      .hezuo_right {
        width: 360px;
        padding-bottom: 10px;
        border-bottom: 2px solid #E3E3E3;
        h1 {
          font-size: 30px;
          color: #353535;
          font-weight: bold;
          margin-top: 10px;
        }
        p {
          color: #666666;
          font-size: 24px;
          margin-top: 10px;
          font-weight: bold;
        }
        span {
          font-weight: bold;
          color: #333;
        }
      }
    }
  }
</style>