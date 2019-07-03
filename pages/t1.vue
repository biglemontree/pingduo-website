<template>
  <div>
    <div class="container is-flex-desktop justify-center item-wrap">
      <div class="left-desc">
        <div>
          <img src="~/assets/t1/i_t1.png" alt />
        </div>
        <div class="lock-desc">全自动,更未来</div>
        <p class="desc fs-24px">高清LED显示屏 | 瑞典FPC指纹头 | 人体工程学把手 | 隐藏式钥匙孔</p>
        <div class="icons flex">
          <div class="has-text-centered">
            <img src="~/assets/p1/icon_zwsb.png" style="magin:auto;" alt />
            <div class="fs-16px">指纹开锁</div>
          </div>
          <div class="icon-item has-text-centered">
            <img src="~/assets/m1/i_2.png" style="magin:auto;" alt />
            <div class="fs-16px">密码开锁</div>
          </div>
          <div class="icon-item has-text-centered">
            <img src="~/assets/m1/i_3.png" style="magin:auto;" alt />
            <div class="fs-16px">钥匙开锁</div>
          </div>
        </div>
      </div>
      <div class="pic-neck has-text-centered">
        <img class="pic-m1" src="~/assets/index/t1.png" alt />
      </div>
    </div>
    <div class="bg-1">
      <div class="container">
        <div class="word-title has-text-centered">
          <h2>高精度外观设计</h2>
          <p class="fs-26px">
            T1的设计方案是由获得多项红点奖的设计师亲自操刀设计，表面采用IMD加工工艺，坚固防抗腐
            蚀且耐用
          </p>
        </div>
      </div>
    </div>
    <div class="bg-2">
      <div class="container">
        <div class="word-title has-text-centered">
          <h2>人体工程学设计</h2>
          <p class="fs-26px">
            相比传统显示屏视角设计，T1根据人体工程学原理，以115°角倾斜设计，让用户体验起来更舒服，
            从每个细节把控，让智能锁更未来
          </p>
        </div>
      </div>
    </div>
    <div class="bg-3">
      <div class="container">
        <div class="word-title has-text-centered">
          <h2>轻松解锁，一气呵成</h2>
          <p class="fs-26px">
            T1采用瑞典FPC半导体传感器轻松解锁，一气呵成。开门无需手动推拉把手，指纹一触即开，
            从未如此快捷
          </p>
        </div>
      </div>
    </div>

    <div class="bg-4" style="padding-top: 71px">
      <div class="word-title has-text-centered">
        <h2>可拆卸锂电池</h2>
        <p class="fs-26px">采用2700毫安可拆卸锂电池，使用时间更长，充电更方便。让智能，不断电</p>
      </div>
    </div>
    <div class="bg-5">
      <div class="has-text-centered" style="padding:120px 0 0px;">
        <div class="word-title">
          <h2>C级锁芯 防技术开启</h2>
          <p class="fs-26px">
            采用C级防盗锁芯,有效防止270分钟内技术开启，隐藏式锁孔设计美观大方，保障家庭的
            安全与美好
          </p>
        </div>
      </div>
    </div>
    <div class="bg-6" style="padding:145px 0 0;">
        <img class="container" src="~/assets/t1/bg_6.png" alt="">
    </div>
  </div>
</template>

<style lang="less" scoped>
img {
  display: block;
}
@media screen and (min-width: 1024px) {
  .container {
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

  .bg-1 {
    height: 1079px;
  }
  .bg-2 {
    height: 1106px;
    .up-arrow {
      color: #1670eb;
      font-size: 28px;
    }
    .percent {
      font-size: 72px;
      color: #1670eb;
    }
  }
  .bg-3 {
    height: 1249px;
    .icon-tip {
      margin-left: 155px;
      .circle-c {
        font-size: 32px;
        z-index: 1000;
        border-radius: 50%;
        width: 89px;
        height: 89px;
        border: 2px solid rgba(255, 255, 255, 1);
        margin-bottom: 29px;
      }
    }
  }
  .bg-4 {
    height: 1144px;
  }
  .bg-5 {
    height: 1089px;
  }
}
@media screen and (max-width: 1023px) {
  .pic-m1 {
    margin-top: 30px;
  }
}
.item-wrap {
  margin-bottom: 120px;
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
  .section {
    .container {
    }
  }
  .pic-m1 {
    width: 185px;
    height: 333px;
  }
}

.bg-1 {
  background: url("../assets/t1/bg_1.png");
}
.bg-2 {
  background: url("../assets/t1/bg_2.png");
}
.bg-3 {
  background: url("../assets/t1/bg_3.png");
}
.bg-4 {
  background: url("../assets/t1/bg_4.png");
}
.bg-5 {
  background: url("../assets/t1/bg_5.png");
}
// .bg-6 {
//   background: url("../assets/t1/bg_6.png");
// }

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
</style>
