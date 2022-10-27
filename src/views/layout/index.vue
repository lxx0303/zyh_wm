<template>
  <div class="layout-container">
    <router-view />
    <van-tabbar class="layout-tabbar" route>
      <van-tabbar-item to="/">
      <!-- <van-icon name="chat-o" badge="99+" /> -->
        <van-icon slot="icon" class="iconfont icon-gongwenbao" dot badge="111"></van-icon>
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
  name: 'LayoutIndex',
  components: {},
  props: {},
  data () {
    return {
    }
  },
  computed: {},
  watch: {},
  created () {},
  mounted () {},
  methods: {}
}
</script>

<style scoped lang="less">
.layout-container {
  .layout-tabbar {
    display: flex;
    span.text {
      font-size: 12px;
      color: #333;
    }
    .iconfont{
      font-size: 24px;
      color: #333;
    }
    .icon-xiaoxi{
      font-size: 28px;
    }
  }
}
</style>
