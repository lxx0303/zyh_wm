<template>
  <div class="home-container">
    <div class="top">
      <van-search
        shape="round"
        background="#00669a"
        placeholder="搜索地点、时间"
      />
      <div>
        <van-grid class="select-pic">
          <van-grid-item icon="clock-o" text="时间" />
          <van-grid-item icon="location-o" text="地点" />
          <van-grid-item icon="notes-o" text="岗位" />
        </van-grid>
      </div>
    </div>

    <div class="main">
      <div class="list-time">
        <div class="time">
          <span>时间</span>
          <van-icon name="down" class="icon" />
          <div class="line"></div>
        </div>
        <div class="text">
          <div class="text-o">
            <div class="text-t">图书管理员</div>
            <div class="text-time">2022-08-12</div>
          </div>
          <div class="text-main">
            <div class="text-main-left">
              <div class="text-main-left-name">
                <div>工作时长</div>
                <div>工作地点</div>
                <div>联系人</div>
              </div>
              <div>
                <div>4小时/天</div>
                <div>第一图书馆</div>
                <div>第一图书馆办公室</div>
              </div>
            </div>
            <div class="text-main-right">
              <button>点击了解</button>
            </div>
          </div>
        </div>
      </div>
      <div class="list-time" v-for="(item, i) in 4" :key="i">
        <div class="text">
          <div class="text-o">
            <div class="text-t">图书管理员</div>
            <div class="text-time">2022-08-12</div>
          </div>
          <div class="text-main">
            <div class="text-main-left">
              <div class="text-main-left-name">
                <div>工作时长</div>
                <div>工作地点</div>
                <div>联系人</div>
              </div>
              <div>
                <div>4小时/天</div>
                <div>第一图书馆</div>
                <div>第一图书馆办公室</div>
              </div>
            </div>
            <div class="text-main-right">
              <button>点击了解</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomePage",
  components: {},
  props: {},
  data() {
    return {};
  },
  computed: {},
  watch: {},
  created() {},
  mounted() {},
  methods: {},
};
</script>

<style scoped lang="less">
.home-container {
  margin-bottom: 52px;
}
.top {
  width: 100%;
  height: 140px;
  // background-color: pink;
  margin-bottom: 10px;

  .select-pic {
    display: flex;
    justify-content: space-between;
  }
  [class*=van-hairline]::after{
    border: 0 ;
  }
}
.main {
  .list-time {
    width: 100%;
    // height: 140px;
    // background-color: skyblue;
    margin-bottom: 10px;
    padding: 25px 20px 10px 15px;
    .time {
      margin-bottom: 20px;
      span {
        font-size: 24px;
      }
      .icon {
        margin-left: 14px;
        font-size: 22px;
        color: #8d8d8d;
      }
      .line {
        width: 280px;
        height: 1px;
        background-color: #d9d9d9;
        margin: 20px auto;
      }
    }
    .text-o {
      display: flex;
      justify-content: space-between;
    }
    .text-t {
      font-weight: 700;
      font-size: 18px;
    }
    .text-time {
      margin-right: 50px;
      font-weight: 700;
      font-size: 16px;
      color: #00669a;
    }
    .text-main{
      display: flex;
      justify-content: space-between;
    }
    .text-main-left {
      margin-top: 10px;
      display: flex;
      font-size: 16px;
      color: #bebebe;
      .text-main-left-name {
        margin-right: 15px;
      }
    }
    .text-main-right{
      button{
        margin-right: 50px;
        margin-top: 46px;
        width: 75px;
        height: 25px;
        font-size: 14px;
        color: #ffffff;
        background-color: #00669a;
        border: 0;
        border-radius: 3px;
      }
    }
  }
  .list {
    width: 100%;
    // height: 130px;
    background-color: skyblue;
    margin-bottom: 10px;
    padding: 10px 20px 10px 15px;
  }

}

</style>
