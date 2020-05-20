<template>
  <div class="puyuan">
    <div class="puyuan_search">
      <van-search left-icon="http://wynode.com/haopuduo/最新铺源icon/icon-py-search@3x.png" shape="round" placeholder="请输入小区或地址或店名" />
    </div>
    <div class="puyuan_top">
      <div class="py_top_left">
        <van-dropdown-menu>
          <van-dropdown-item title="区域">
            <van-tree-select :items="items" :main-active-index="mainActiveIndex" :active-id="activeId" />
          </van-dropdown-item>
          <van-dropdown-item title="行业">
            <van-tree-select :items="items" :main-active-index="mainActiveIndex" :active-id="activeId" />
          </van-dropdown-item>
          <van-dropdown-item title="价格">
            <van-tree-select :items="items" :main-active-index="mainActiveIndex" :active-id="activeId" />
          </van-dropdown-item>
          <van-dropdown-item title="更多">
            <van-tree-select :items="items" :main-active-index="mainActiveIndex" :active-id="activeId" />
          </van-dropdown-item>
        </van-dropdown-menu>
      </div>
      <div class="py_top_right">
        <img src="http://wynode.com/haopuduo/最新铺源icon/icon-py-px@3x.png" alt="" />
      </div>
    </div>
    <div class="py_bottom" @click="goshangpuxiangqin">
      <secitem v-for="item in 10" :key="item" :btntype="'default'"></secitem>
    </div>
  </div>
</template>

<script>
  import secitem from '@/components/secitem'
  export default {
    components: {
      secitem,
    },
    data() {
      return {
        mainActiveIndex: 0,
        activeId: 1,
        value1: "a",
        itemTitle: "筛选",
        options1: [{
          text: "默认排序",
          value: "a"
        }],
        items: [{
            text: "浦东",
            children: [{
                text: "北蔡",
                id: 1,
              },
              {
                text: "碧云",
                id: 2,
              },
              {
                text: "曹路",
                id: 3,
              },
            ],
          },
          {
            text: "徐汇",
            children: [{
                text: "测试1",
                id: 1,
              },
              {
                text: "测试2",
                id: 2,
              },
              {
                text: "测试3",
                id: 3,
              },
            ],
          },
          {
            text: "长宁",
            children: [{
                text: "测试1",
                id: 1,
              },
              {
                text: "测试1",
                id: 2,
              },
              {
                text: "测试1",
                id: 3,
              },
            ],
          },
          {
            text: "静安",
            children: [{
                text: "测试1",
                id: 1,
              },
              {
                text: "测试1",
                id: 2,
              },
              {
                text: "测试1",
                id: 3,
              },
            ],
          },
        ],
      };
    },
    methods: {
      goshangpuxiangqin() {
        const url = "/pages/shangpuxiangqin/main";
        mpvue.navigateTo({
          url
        });
      },
    },
  };
</script>

<style lang="scss">
  .py_bottom {
    width: 690px;
    margin: 0 auto;
    margin-top: var(--test-margin-top, 50px);
  }
  .puyuan {
    width: 100%;
    --search-background-color: #fff;
    --test-margin-top: 10px;
    --cell-line-height: 44px;
  }
  .puyuan .van-dropdown-menu {
    margin-left: -20px;
    height: 80px;
  }
  .puyuan_top {
    width: 710px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-bottom: 1px solid #e3e3e3;
    padding-right: 20px;
  }
  .py_top_right {
    border-left: 1px solid #e3e3e3;
    padding-left: 28px;
  }
  .py_top_left {
    width: 622px;
    font-size: 28px;
  }
  .py_top_left .van-dropdown-menu__title {
    font-size: 28px;
    line-height: 28px;
  }
  .py_top_right img {
    width: 32px;
    height: 26px;
  }
  .puyuan_search {
    width: 720px;
    margin: 0 auto;
    margin-top: 10px;
    margin-bottom: 20px;
    .van-icon--image {
      width: 32px;
      height: 32px;
    }
  }
  .puyuan_search .van-search {
    width: 710px;
    height: 58px;
    background: #fff;
  }
  .puyuan_search .van-search__content {
    border-radius: 34px;
    border: 1px solid #ddd;
  }
  .puyuan_search .van-search__field {
    height: 58px;
  }
  .puyuan_search .van-field__input {
    font-size: 24px;
    line-height: 48px;
  }
  .puyuan_search .van-cell__left-icon-wrap {
    width: 40px;
    height: 48px;
    line-height: 48px;
  }
  // .puyuan_search .van-cell {
  //   background: #fff;
  // }
  .puyuan_search .van-icon__image {
    width: 32px;
    height: 32px;
  }
</style>
