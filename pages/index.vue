<template>
  <div>
    <div class="hero">
      <div class="container  has-text-centered is-hidden-mobile">
        <div class="top-lock flex justify-between items-center ">
          <div class="center">
            <img src="~/assets/index/icon_m1.png" alt>
            <div>智能指纹锁 M1</div>
          </div>
          <div class="">
            <img src="~/assets/index/icon_p1.png" alt>
            <div>智能指纹锁 P1</div>
          </div>
          <div class="">
            <img src="~/assets/index/icon_t1.png" alt>
            <div>智能指纹锁 t1</div>
          </div>
          <div class="">
            <img src="~/assets/index/icon_pj.png" alt>
            <div>配件</div>
          </div>
        </div>
      </div>
    </div>
    <div class="bg-f2 gray-block is-hidden-mobile"></div>
    <div class="section lock-body">
      <div class="container">
        <div class="clear-float">
          <div class="left has-text-centered">
            <div class="smart-lock flex items-center">
              <h2 >智能门锁</h2>
              <img src="~/assets/index/tb_m1.png" alt>
            </div>
            <div>开启瞬间,点亮生活</div>
            <p class="desc">
              全自动智能锁M1，采用手机CNC工艺，双重专利认证，结合
              人工智能算法，让生活更便捷。
            </p>
            <img src="~/assets/index/icon_pj.png" alt>
            <a href>进一步了解</a>
          </div>
          <div class="right">
            <img src="~/assets/index/m1.png" alt>
            <!-- <div>配件</div> -->
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="columns">
        <div class="column">
          <img src="~/assets/index/icon_m1.png" alt>
          <!-- <div>智能指纹锁 M1</div> -->
        </div>
        <div class="column">
          <img src="~/assets/index/icon_p1.png" alt>
          <!-- <div>智能指纹锁 P1</div> -->
        </div>
        <div class="column">
          <img src="~/assets/index/icon_t1.png" alt>
          <!-- <div>智能指纹锁 t1</div> -->
        </div>
        <div class="column">
          <img src="~/assets/index/icon_pj.png" alt>
          <!-- <div>配件</div> -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  layout: "default",
  components: {
    Logo
  }
};
</script>

<style lang="less" scoped>
.section {  
  .container {
    width: 222px;
  }
}
.top-lock {
  width: 500px;
  height: 130px;
}
.lock-body {
    .left::after,
    .right::after {
        clear: both;
    }
}
.smart-lock {
    h2 {
        width:192px;
        height:43px;
        font-size:42px;
        font-family:MicrosoftYaHei;
        font-weight:400;
        color:rgba(52,150,246,1);
        line-height:79px;
    }
}
</style>
