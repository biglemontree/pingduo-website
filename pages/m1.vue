<template>
  <div>
    <div class="container is-flex-desktop justify-center item-wrap">
      <div class="left-desc">
        <div>
          <img class="icon-m1" src="~/assets/m1/icon_m1.png" alt>
        </div>
        <div class="lock-desc is-size-2-mobile has-text-centered-mobile">瞬间点亮，开启快捷生活</div>
        <p class="desc fs-24px is-size-5-mobile has-text-centered-mobile">手机CNC工艺 | 无把手设计 | 双重专利认证 | 人工智能算法</p>
        <div class="icons flex">
          <div class="has-text-centered">
            <img src="~/assets/p1/icon_zwsb.png" alt>
            <div class="fs-16px">指纹开锁</div>
          </div>
          <div class="icon-item has-text-centered">
            <img src="~/assets/m1/i_2.png" alt>
            <div class="fs-16px">密码开锁</div>
          </div>
          <div class="icon-item has-text-centered">
            <img src="~/assets/m1/i_3.png" alt>
            <div class="fs-16px">钥匙开锁</div>
          </div>
        </div>
      </div>
      <div class="pic-neck has-text-centered">
        <img class="pic-m1"   src="~/assets/index/m1.png" alt>
      </div>
    </div>
    <div class="bg-1">
      <div class="container">
        <div class="word-title has-text-centered">
          <h2 class="is-size-2-mobile">行业创新的面板对称设计</h2>
          <p class="fs-26px is-size-5-mobile">
            前后面板对称式设计，前后一致，表里如一。突破全自动指纹锁后面板颜值过低的短板，实现高
            颜值与黑科技并存。
          </p>
        </div>
        <div class="rotate-img is-hidden-mobile">
            <img  src="~/assets/m1/1_1.png" alt>
            <img  class="pc-pic" src="~/assets/m1/1_2.png" alt>
            <!-- <img  src="~/assets/m_m1/bg_1.png" alt> -->
        </div>
      </div>
    </div>
    <div class="bg-2">
      <div class="container">
        <div class="word-title has-text-centered">
          <h2 class="is-size-2-mobile">双重认证 防儿童误开功能</h2>
          <p class="fs-26px is-size-5-mobile">室内开门时，需同时碰触背面感应区+按压开锁键，才可开门。以防小孩不小心按压开门键将门误开。</p>
        </div>
      </div>
        <img  class="is-hidden-desktop" src="~/assets/m_m1/bg_2.png" alt>
    </div>
    <div class="bg-3">
      <div class="container">
        <div class="word-title has-text-centered">
          <h2 class="is-size-2-mobile">高亮铝合金曲面边框设计</h2>
          <p class="fs-26px is-size-5-mobile">
            尖端高精度数控车床（ＣＮＣ）加工工艺，高密度表面氧化处理，提升产品耐磨耐腐蚀性，
            整体工艺细节与高端手机一致，突破行业原有水平，无论是在外观或者使用手感上，
            让产品触摸体验更胜一筹。
          </p>
        </div>
      </div>
    </div>
    <div class="bg-4">
      <div class="container">
        <div class="word-title has-text-left" >
          <h2 class="is-size-2-mobile">报警功能</h2>
          <p class="fs-26px is-size-5-mobile">
            当门锁被撬时，门锁自身将发出
            警报，同时将告警信息发送到手
            机的华为智能家居APP上。
          </p>
        </div>
        <div class="flex justify-center is-hidden-mobile">
          <img src="~/assets/m1/4_2.png" alt>
          <div>安全加倍</div>
        </div>
      </div>
    </div>
    <div class="bg-5" style="padding-top: 71px">
      <div class="word-title has-text-centered">
        <h2 class="is-size-2-mobile">虚位密码</h2>
        <p class="fs-26px is-size-5-mobile" style="margin: 70px 0 30px;">
          可有效防止他人通过指纹查看密码痕迹破解密码（比如不方便让同行的亲友看到正确密码，则可
          以输入虚位密码，避免尴尬）
        </p>
        <h3 class="fs-28px" style="margin: 0px 0 30px;">使用方法</h3>
        <div class="flex justify-center">
          <img src="~/assets/m1/5_1.png" alt>
        </div>
        <p class="fs-20px" style="margin: 20px 0 0px;">15位数字内含正确密码</p>
      </div>
    </div>
    <div >
      <img src="~/assets/m1/6_2.png" style="margin: 105px auto 30px;" alt>
      <div class="bg-6">

      </div>
    </div>
  </div>
</template>

<style lang="less" scoped>
img {
  display: block;
}
@media screen and (min-width: 1024px) {
  .container {
    font-size: 0;
    padding-top: 109px;
    justify-content: center;
    // width: 513px;
    .left-desc {
      padding-top: 100px;
      margin-right: 62px;
      width: 700px;
      .icon-item {
        margin-left: 90px;
      }
    }
  }
    .item-wrap {
        margin-bottom: 120px;
    }
    .word-title {
        color: #ffffff;
        h2 {
            font-size: 60px;
            margin: 50px 0 40px;
        }
        p {
            margin-bottom: 87px;
        }
    }
    .bg-1 {
        background: url("../assets/m1/bg_1.png");
        .pc-pic {
            margin-top: 60px;padding-bottom:97px;
        }
    }
  .bg-2 {
    background: url("../assets/m1/2_1.png");
    height: 1106px;
  }
  .bg-3 {
    background: url("../assets/m1/3_1.png");
    height: 1249px;
  }
  .bg-4 {
    background: url("../assets/m1/4_1.png");
    height: 931px;
    .word-title {width: 391px;margin-left: 300px;}
    .flex {width: 391px;margin-left: 300px;}
  }
  .bg-5 {
  background: url("../assets/m1/5_2.png");

    height: 975px;
  }
  .bg-6 {
    height: 842px;
  }
}
@media screen and (max-width: 1023px) {
    .icon-m1 {
        padding-top: 20px;
        width: 70%;
        margin: auto;
    }
    .icons {
        justify-content: center;
        .icon-item {
            margin-left: 40px;
        }
    }
  .pic-m1 {
    margin: 30px auto 0;
  }
  .bg-1 {
    // background: black;
    background: url("../assets/m_m1/bg_1.png");

      min-height: 600px;
  }
  .bg-2 {
      padding: 60px 0 200px;
      background-size:contain;
  }
}

.left-desc {
  .lock-desc {
    font-size: 60px;
    margin: 20px 0 24px;
  }
  .desc {
    margin-bottom: 58px;
  }
}
.pic-m1 {
  width: 370px;
  height: 666px;
}

@media screen and (max-width: 768px) {
  .pic-m1 {
    width: 185px;
    height: 333px;
  }
  h2 {margin-bottom: 20px;}
  .bg-1 {
        padding: 50px 20px 0px;

        background-size: contain;
        background-position: bottom;
  }
    // .bg-1,
    .bg-2,
    .bg-3, 
    .bg-4, 
    .bg-5 {
        padding: 50px 20px 0px;
        min-height: 500px;
        background-size: contain;
        background-position: bottom;
    }
  
    .bg-3 {background: url("../assets/m_m1/bg_3.png") bottom no-repeat ;}
    .bg-4 {background: url("../assets/m_m1/bg_4.png");background-size: 100%;}
    .bg-5 {background: url("../assets/m_m1/bg_5.png");background-size: 100%;}
}
.word-title {
    color: #ffffff;
}

.bg-2 {
  background: url("../assets/m1/2_1.png");
}
.bg-3 {
  min-height: 600px;
  background-size: contain;
//     background-position: bottom;
    background-color: black;
}
.bg-4 {
}
.bg-5 {
}
.bg-6 {
  background: url("../assets/m1/6_1.png");
  background-size: 100%;
}


</style>
