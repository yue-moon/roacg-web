
<template>
  <default-layout>
    <div style="background-color: white; min-height:980px">
      <div id="ro-home-warp">
        <!-- 第一层 内容和讯息-->
        <a-row type="flex" :gutter="[8,8]">
          <!-- 轮播图 -->
          <a-col :span="12">
            <!-- border 没用 艹 -->
            <a-carousel autoplay style="border-radius: 5px">
              <div class="top-home-slide">
                <h3>1</h3>
              </div>
              <div class="top-home-slide">
                <h3>2</h3>
              </div>
              <div class="top-home-slide">
                <h3>3</h3>
              </div>
            </a-carousel>
          </a-col>

          <!-- 讯息 -->
          <a-col :span="12">
            <a-card style="height: 57%"></a-card>
            <div style="height: 3%"></div>
            <a-card style="height: 40%"></a-card>
          </a-col>
        </a-row>

        <!-- 第二层 不知道放啥 先放着 -->
        <a-card
          :loading="true"
          style="height: 360px; margin-top: 16px;padding: 24px;"
        >whatever content</a-card>
      </div>
    </div>
  </default-layout>
</template>


<script>
export default {};
</script>

<style lang="less" scoped>
#ro-home-warp {
  width: 1414px;
  margin: 0 auto;
  padding-top: 16px;

  @media screen and (max-width: 1654px) {
    width: 1198px;
  }

  @media screen and (max-width: 1438px) {
    width: 999px;
  }

  //FIXME 测试用; 撑个页面骨架
  .top-home-slide {
    text-align: center;
    height: 228px;
    line-height: 160px;
    background: #364d79;
    overflow: hidden;
  }
  .top-home-slide h3 {
    color: #fff;
  }
}
</style>