<template>
  <div>
    <div class="hero">
      <div class="container  has-text-centered is-hidden-mobile">
        <div class="top-lock flex justify-between items-center ">
            <nuxt-link to="/m1">
                <div class="center">
                    <img src="~/assets/index/icon_m1.png" alt>
                    <div>智能指纹锁 M1</div>
                </div>
            </nuxt-link>
            <nuxt-link to="/p1">
                <div class="">
                    <img src="~/assets/index/icon_p1.png" alt>
                    <div>智能指纹锁 P1</div>
                </div>
            </nuxt-link>
          <nuxt-link to="/t1">
            <div class="">
                <img src="~/assets/index/icon_t1.png" alt>
                <div>智能指纹锁 t1</div>
            </div>
          </nuxt-link>
          <!-- <div class="">
            <img src="~/assets/index/icon_pj.png" alt>
            <div>配件</div>
          </div> -->
        </div>
      </div>
    </div>
    <div class="bg-f2 gray-block is-hidden-mobile"></div>
    <div class=" lock-body">
      <div class="container px-20px">
        <div class="is-flex-desktop justify-center item-wrap item-1">
          <div class="m1-left left-desc has-text-centered">
            <div class="smart-lock flex items-center justify-center">
              <h2 class="mr-22px is-size-3-mobile">智能门锁</h2>
              <img src="~/assets/index/tb_m1.png" alt>
            </div>
            <div class="lock-desc is-size-3-mobile">开启瞬间,点亮生活</div>
            <p class="desc fs-20px is-size-5-mobile">
              全自动智能锁M1，采用手机CNC工艺，双重专利认证，结合人工智能算法，让生活更便捷。
            </p>
            <img class="goods" src="~/assets/index/tp_jdj.png" alt>
            <div class="know-more">
                <nuxt-link class="navbar-item nuxt-link-active flex justify-center" to="/m1">进一步了解</nuxt-link>
                <span class="arrow"></span>
            </div>
          </div>
          <div class="pic-neck has-text-centered">
            <img class="pic-m1" src="~/assets/index/m1.png"  alt>
          </div>
        </div>
      </div>
        <div class="px-20px is-flex-desktop justify-center item-wrap bg-f2">
          <div class="left-desc has-text-centered p1-left">
            <div class="smart-lock flex items-center justify-center">
              <h2 class="mr-22px is-size-3-mobile">智能门锁</h2>
              <img src="~/assets/index/tp_p1.png" alt>
            </div>
            <div class="lock-desc is-size-3-mobile">如此快捷,一握即开</div>
            <p class="desc fs-18px is-size-5-mobile">智能指纹锁P1，创新门把手设计，超长续航能力，多种开门方式，轻松满足每个家庭成员需求。
            </p>
            <div class="know-more">
                <nuxt-link class="navbar-item nuxt-link-active flex justify-center" to="/p1">进一步了解</nuxt-link>
                <span class="arrow"></span>
            </div>
          </div>
          <div class="pic-neck has-text-centered">
            <img class="pic-p1" src="~/assets/index/p1.png"  alt>
          </div>
        </div>
        <div class="px-20px is-flex-desktop justify-center item-wrap">
          <div class="t1-left left-desc has-text-centered">
            <div class="smart-lock flex items-center justify-center">
              <h2 class="mr-22px is-size-3-mobile">智能门锁</h2>
              <img src="~/assets/index/tp_t1.png" alt>
            </div>
            <div class="lock-desc is-size-3-mobile">全自动,更未来</div>
            <p class="desc fs-20px is-size-5-mobile">全自动智能锁T1，采用imd加工工艺，高安全级别锁芯，高适配率无需改孔，想装就装。
            </p>
            <div class="know-more">
                <nuxt-link class="navbar-item nuxt-link-active flex justify-center" to="/t1">进一步了解</nuxt-link>
                <span class="arrow"></span>
            </div>
          </div>
          <div class="pic-neck has-text-centered">
            <img class="pic-t1" src="~/assets/index/t1.png"  alt>
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
// Arrow
// -------------------------
._setArrow(@arrowsize, @borderColor, @borderWidth){
    display: inline-block;
    height: @arrowsize;
    width: @arrowsize;
    border-width: @borderWidth @borderWidth 0 0;
    border-color: @borderColor;
    border-style: solid;
}
.setArrow(@direction, @arrowsize, @borderColor,@borderWidth) when (@direction = right) {
    ._setArrow(@arrowsize, @borderColor, @borderWidth);
    transform: matrix(0.71,0.71,-0.71,0.71,0,0); // rotate(45deg);

    position: relative;
}
@media screen and (min-width: 1024px) {
    .container {
        justify-content: center;
        // width: 513px;
        .left-desc {
            padding-top: 100px;
            margin-right: 62px;
        }
        .pic-p1 {
            margin-right: 36px;
        }
    }
    .item-wrap {
        margin-bottom: 100px;
    }
    .item-1 {
        background: url('../assets/index/bg_logo.png') no-repeat center;
    }
    .m1-left {
        width: 540px;
    }
    .p1-left {
        order: 2;
        width: 629px;
        margin-left: 20px;
    }
    .t1-left {
        width: 529px;
        margin-right: 40px;
    }
}
@media screen and (max-width: 1023px) {
    .pic-m1 {
        margin-top: 30px;
    }
}
.item-wrap {
    padding: 86px 20px 80px;
}
.left-desc {
    .lock-desc {
        font-size: 48px;
        margin: 28px 0 20px;
    }
    .goods {
        margin: 31px 0 0;
    }
}
.pic-m1 {
    width: 370px;
    height: 666px;
}
.pic-p1 {
    width: 323px;
    height: 674px;
}
.pic-t1 {
    width: 422px;
    height: 671px;
}
.know-more {
    display: flex;
    justify-content: center;
    align-items: center;
    a {
        color: #1AA0FB !important;
        text-align: center;
        &::after {
        .setArrow(right,10px,#00A8EC,2px)

        }
    }
    .arrow {
        .setArrow(right,10px,#00A8EC,2px)

    }
    font-size: 24px;
    margin: 60px 0 35px;
}
@media screen and (max-width: 768px) { 
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
    .smart-lock {
        img {
            width: 52px;
        }
    }
}
.top-lock {
  width: 500px;
  height: 130px;
  img {
      height: 64px;
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
        font-size:42px;
        color:rgba(52,150,246,1);
        margin-right: 22px;
    }
}
</style>
