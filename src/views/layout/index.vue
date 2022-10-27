<template>
  <div class="layout-container">
    <router-view />
    <van-tabbar
      class="layout-tabbar"
      route
      fixed
    >
      <van-tabbar-item to="/home">
        <van-icon
          slot="icon"
          class="iconfont icon-gongwenbao"
          info="new"
        ></van-icon>
        <span class="text">工作</span>
      </van-tabbar-item>
      <van-tabbar-item to="/message">
        <i slot="icon" class="iconfont icon-xiaoxi"></i>
        <span class="text">消息</span>
      </van-tabbar-item>
      <van-tabbar-item to="/my">
        <i slot="icon" class="iconfont icon-wode"></i>
        <span class="text">我的</span>
      </van-tabbar-item>
    </van-tabbar>
  </div>
</template>

<script>
export default {
  name: "LayoutIndex",
  components: {},
  props: {},
  data() {
    return {
    };
  },
  computed: {},
  watch: {},
  created() {},
  mounted() {},
  methods: {},
};
</script>

<style scoped lang="less">
.layout-container {
  .layout-tabbar {
    span.text {
      font-size: 12px;
    }
    .iconfont {
      font-size: 24px;
    }
    .icon-xiaoxi {
      font-size: 28px;
    }
  }
}
</style>
