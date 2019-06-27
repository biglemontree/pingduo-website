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
        <div class="is-flex-desktop justify-center item-wrap">
          <div class="left-desc has-text-centered">
            <div class="smart-lock flex items-center justify-center">
              <h2 class="mr-22px">智能门锁</h2>
              <img src="~/assets/index/tb_m1.png" alt>
            </div>
            <div class="lock-desc">开启瞬间,点亮生活</div>
            <p class="desc fs-9px">
              全自动智能锁M1，采用手机CNC工艺，双重专利认证，结合
              人工智能算法，让生活更便捷。
            </p>
            <img class="goods" src="~/assets/index/tp_jdj.png" alt>
            <div class="know-more">
                <a href>进一步了解</a>
            </div>
          </div>
          <div class="pic-neck has-text-centered">
            <img class="pic-m1" src="~/assets/index/m1.png"  alt>
          </div>
        </div>
        <div class="is-flex-desktop justify-center item-wrap">
          <div class="left-desc has-text-centered p1-left">
            <div class="smart-lock flex items-center justify-center">
              <h2 class="mr-22px">智能门锁</h2>
              <img src="~/assets/index/tp_p1.png" alt>
            </div>
            <div class="lock-desc">如此快捷,一握即开</div>
            <p class="desc fs-9px">智能指纹锁P1，创新门把手设计，超长续航能力，多种开门方式，轻松满足每个家庭成员需求。
            </p>
            <div class="know-more">
                <a href>进一步了解</a>
            </div>
          </div>
          <div class="pic-neck has-text-centered">
            <img class="pic-p1" src="~/assets/index/p1.png"  alt>
          </div>
        </div>
        <div class="is-flex-desktop justify-center item-wrap">
          <div class="left-desc has-text-centered">
            <div class="smart-lock flex items-center justify-center">
              <h2 class="mr-22px">智能门锁</h2>
              <img src="~/assets/index/tp_t1.png" alt>
            </div>
            <div class="lock-desc">全自动,更未来</div>
            <p class="desc fs-9px">全自动智能锁T1，采用imd加工工艺，高安全级别锁芯，高适配率无需改孔，想装就装。
            </p>
            <div class="know-more">
                <a href>进一步了解</a>
            </div>
          </div>
          <div class="pic-neck has-text-centered">
            <img class="pic-t1" src="~/assets/index/t1.png"  alt>
          </div>
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
@media screen and (min-width: 1024px) {
    .container {
        justify-content: center;
        // width: 513px;
        .left-desc {
            padding-top: 75px;
            margin-right: 36px;
            width: 265px;
        }
        .p1-left {
            order: 2;
        }
        .pic-p1 {
            margin-right: 36px;
        }
    }
}
@media screen and (max-width: 1023px) {
    .pic-m1 {
        margin-top: 30px;
    }
}
.item-wrap {
    margin-bottom: 100px;
}
.left-desc {
    .lock-desc {
        font-size: 28px;
        margin: 14px 0 17px;
    }
    .goods {
        margin: 13px 0 34px;
    }
}
.pic-m1 {
    width: 185px;
    height: 333px;
}
.pic-p1 {
    width: 162px;
    height: 337px;
}
.pic-t1 {
    width: 211px;
    height: 336px;
}
.know-more {
    color: #1AA0FB;
    font-size: 12px;
    margin: 41px 0 35px;
}
@media screen and (max-width: 768px) { 
    .section {  
        .container {
            width: 222px;
        }
    }
}
.top-lock {
  width: 500px;
  height: 65px;
  img {
      height: 32px;
  }
}
.lock-body {
    .left::after,
    .right::after {
        clear: both;
    }
}
.smart-lock {
    h2 {
        font-size:21px;
        color:rgba(52,150,246,1);
        margin-right: 11px;
    }
}
</style>
