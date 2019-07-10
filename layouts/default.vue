<template>
  <div>
    <div class="sticky-nav">
      <nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation">
        <div class="container">
          <div class="navbar-brand">
            <a
              role="button"
              class="navbar-burger burger is-pulled-left"
              aria-label="menu"
              aria-expanded="false"
              data-target="navbarBasicExample"
            >
              <span aria-hidden="true"></span>
              <span aria-hidden="true"></span>
              <span aria-hidden="true"></span>
            </a>
            <a class="navbar-item mobile-logo is-pulled-left-desktop">
              <img src="~/assets/logo.png" width="112" height="28" />
            </a>
            <div class="navbar-item is-pulled-right-mobile is-hidden-desktop">
              <div class="buttons">
                <a class="button online-buy">在线购买</a>
              </div>
            </div>
          </div>
          <div id="navbarBasicExample" class="navbar-menu">
            <div class="navbar-end">
              <p class="navbar-item nuxt-link-active" to="/">智能门锁
                <ul class="menu-list is-hidden-desktop" >
                    <li class="mt-18px">
                    <a href="./m1">智能指纹锁M1</a>
                    </li>
                    <li>
                    <a href="./p1">智能指纹锁P1</a>
                    </li>
                    <li>
                    <a href="./t1">智能指纹锁T1</a>
                    </li>
                </ul>
              </p>
              <p class="navbar-item" to="/aboutus/company-produce">关于我们
                <ul class="menu-list is-hidden-desktop" >
                    <li class="mt-18px">
                    <a href="./aboutus/company-produce">公司简介</a>
                    </li>
                    <li>
                    <a href="./aboutus/brand-history">品牌故事</a>
                    </li>
                    <li>
                    <a href="./aboutus/pd-only">专利声明</a>
                    </li>
                    <li>
                    <a href="./aboutus/service">售后服务</a>
                    </li>
                </ul>
              </p>
              <nuxt-link class="navbar-item" to="/join">品牌加盟</nuxt-link>
              <nuxt-link class="navbar-item down-app" to="/">
                下载APP
                <div class="down-qrcode">
                  <img src="~/assets/footer/home.png" alt />
                  <img src="~/assets/footer/qr-house.png" alt />
                </div>
              </nuxt-link>
              <div class="navbar-item is-hidden-mobile">
                <div class="buttons">
                  <a class="button online-buy">在线购买</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </nav>
    </div>
    <nuxt />

    <footer class="footer bg-f2">
      <div class="container is-hidden-touch">
        <div class="content columns has-text-lefted">
          <div class="column">
            <div class="title">
              智能门锁
            </div>
            <p><a href>M1</a></p>
            <p>P1</p>
            <p>T1</p>
            <!-- <p>H1</p> -->
            <!-- <p>配件</p> -->
          </div>
          <div class="column">
            <div class="title">关于我们</div>
            <p>
              <a href>公司简介</a>
            </p>
            <p>品牌故事</p>
            <p>专利声明</p>
            <p>售后服务</p>
          </div>
          <div class="column">
            <div class="title">品牌加盟</div>
            <p>加盟</p>
          </div>
          <div class="column is-4 relative">
            <div class="title">APP下载</div>
            <div class="app-qr">
              <img class src="~/assets/footer/home.png" alt />
              <img class src="~/assets/footer/qr-house.png" alt />
            </div>
          </div>
          <div class="column has-text-centered">
            <div class="title">关注公众号</div>
            <div>
              <img src="~/assets/footer/qr-pd.png" alt />
            </div>
            <p>PINTOS 服务公众号</p>
          </div>
        </div>
        <div class="columns copy">
          <p class="column">©2017 PINTOS.ALL right reserved. 粤ICP备171758560号-1</p>
          <p class="column">深圳市几何科技有限公司</p>
          <p class="column tel">400 858 6766</p>
        </div>
      </div>
      <aside class="menu is-mobile is-hidden-desktop ">
        <p class="menu-label">
          <img src="~/assets/logo_b.png" width="112" height="28" />
        </p>
        <div class="menu-label is-size-5-mobile" @click="showIem(1)">
          <div class="main-line">
            智能门锁
            <span class="close"></span>
          </div>
          <ul class="menu-list" v-show="footerItm==1">
            <li class="mt-18px">
              <a href="./m1">M1</a>
            </li>
            <li>
              <a href="./p1">P1</a>
            </li>
            <li>
              <a href="./t1">T1</a>
            </li>
            <li>
              <a href="./h1">H1</a>
            </li>
          </ul>
        </div>
        <div class="menu-label is-size-5-mobile" @click="showIem(2)">
          <div class="main-line">
            关于我们
            <span :class="['close', footerItm==2 && 'open']"></span>
          </div>

          <ul class="menu-list" v-show="footerItm==2">
            <li class="mt-18px">
              <a href="./aboutus/company-produce">公司简介</a>
            </li>
            <li>
              <a href="./aboutus/brand-history">品牌故事</a>
            </li>
            <li>
              <a href="./aboutus/pd-only">专利声明</a>
            </li>
            <li>
              <a href="./aboutus/service">售后服务</a>
            </li>
          </ul>
        </div>
        <p class="menu-label is-size-5-mobile" @click="showIem(3)">品牌加盟</p>
        <!-- <ul class="menu-list">
          <li>
            <a>加盟</a>
          </li>
        </ul>-->
        <p class="menu-label  is-size-5-mobile">APP下载</p>
        <div class="is-size-5-mobile copy-bottom">
          <p class="">深圳市几何科技有限公司</p>
          <p class=" ">400 858 6766</p>
        </div>
        <p class="copy-right">©2017 PINTOS.ALL right reserved. 粤ICP备171758560号-1</p>
      </aside>
    </footer>
  </div>
</template>


<style scoped lang="less">
.navbar {
  background: #3e3e3e;
  height: 60px;
  .container {
    height: 100%;
  }
}
.navbar-brand,
.navbar-tabs {
  height: 60px;
}
.navbar-burger {
  color: #fff;
}
.navbar-burger {
  height: 100%;
}
.navbar-item {
  color: #888;
  font-size: 18px;
  margin-right: 55px;
  img {
    max-height: none;
  }
}
.down-app {
  position: relative;
  .down-qrcode {
    position: absolute;
    // height: 0px;
    img {
      display: none;
    }
  }
}
.down-app:hover {
  .down-qrcode {
    width: 270px;
    top: 70px;
    img {
      display: inline-block;
    }
  }
}
.online-buy {
  width: 100px;
  height: 29px;
  color: #fff;
  border: none;
  background: rgba(54, 155, 250, 1);
  border-radius: 50px;
}
.footer .title {
  font-size: 8px;
  color: rgba(0, 0, 0, 1);
}
.footer p {
  color: #838383;
}
.content {
  padding-bottom: 14px;
  border-bottom: 1px solid #dadada;
}
.app-qr img {
  width: 124px;
  height: 124px;
  margin-right: 16px;
}
.copy .tel {
  font-size: 15px;
  font-weight: 500;
  color: rgba(106, 106, 106, 1);
}
aside {
  .menu-label {
    border-bottom: 1px solid #eeeeee;
    margin: 0;
    padding: 20px 0;
    .main-line {
      display: flex;
      align-items: center;
      justify-content: space-between;
      .close {
        display: inline-block;
        width: 18px;
        height: 2px;
        background: #838383;
        transform: rotate(0deg);
        &::after {
          content: "";
          display: block;
          width: 18px;
          height: 2px;
          background: #838383;
          transform: rotate(-90deg);
        }
      }
      .open {
        transform: rotate(45deg);
      }
    }
  }
}

@media screen and(max-width: 1023px) {
  .navbar-brand {
    display: flex;
    justify-content: space-between;
    .navbar-burger {
      margin-left: 0;
    }
    .mobile-logo {
      margin-left: 10%;
    }
    .navbar-item {
      margin-right: 0;
      .online-buy {
        width: 80px;
      }
    }
  }
  .copy-bottom {
      margin: 10px 0 20px;
      display: flex;
      justify-content: space-between;
      .copy-right {font-size: 8px !important;}
  }
}
</style>

<script type="text/javascript">
export default {
  layout: "default",
  components: {},
  data() {
    return {
      footerItm: 0
    };
  },
  methods: {
    showIem(i) {
      if (this.footerItm === i) {
        this.footerItm = 0;
        return;
      }
      this.footerItm = i;
    }
  },
  mounted() {
    // Get all "navbar-burger" elements
    const $navbarBurgers = Array.prototype.slice.call(
      document.querySelectorAll(".navbar-burger"),
      0
    );

    // Check if there are any navbar burgers
    if ($navbarBurgers.length > 0) {
      // Add a click event on each of them
      $navbarBurgers.forEach(el => {
        el.addEventListener("click", () => {
          // Get the target from the "data-target" attribute
          const target = el.dataset.target;
          const $target = document.getElementById(target);

          // Toggle the "is-active" class on both the "navbar-burger" and the "navbar-menu"
          el.classList.toggle("is-active");
          $target.classList.toggle("is-active");
        });
      });
    }
  }
};
</script>
