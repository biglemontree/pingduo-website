<template>
  <div>
    <div >
      <nav class="navbar" role="navigation" aria-label="main navigation">
        <div class="container">
          <div class="navbar-brand">
            <a class="navbar-item" >
              <img src="~/assets/logo.png" width="112" height="28">
            </a>

            <a
              role="button"
              class="navbar-burger burger"
              aria-label="menu"
              aria-expanded="false"
              data-target="navbarBasicExample"
            >
              <span aria-hidden="true"></span>
              <span aria-hidden="true"></span>
              <span aria-hidden="true"></span>
            </a>
          </div>

          <div id="navbarBasicExample" class="navbar-menu">
            <div class="navbar-end">
              <nuxt-link class="navbar-item nuxt-link-active" to="/">智能门锁</nuxt-link>
              <nuxt-link class="navbar-item" to="/aboutus/company-produce">关于我们</nuxt-link>
              <nuxt-link class="navbar-item" to="/join">品牌加盟</nuxt-link>
              <nuxt-link class="navbar-item" to="/">下载APP</nuxt-link>
              <div class="navbar-item">
                <div class="buttons">
                  <a class="button online-buy">在线购买</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </nav>
    </div>
    <nuxt/>

    <footer class="footer bg-f2">
        <div class="container is-hidden-touch">
            <div class="content columns has-text-lefted ">
                <div class="column">
                <div class="title">智能门锁</div>
                <p>M1</p>
                <p>P1</p>
                <p>T1</p>
                <p>H1</p>
                <p>配件</p>
                </div>
                <div class="column">
                <div class="title">关于我们</div>
                <p>
                    <a href="">公司简介</a></p>
                <p>品牌故事</p>
                <p>专利声明</p>
                <p>售后服务</p>
                </div>
                <div class="column">
                <div class="title">品牌加盟</div>
                <p>加盟</p>
                </div>
                <div class="column is-4">
                    <div class="title">APP下载</div>
                    <div class="app-qr flex">
                        
                        <img class="" src="~/assets/footer/home.png" alt="">
                        <img class="" src="~/assets/footer/qr-house.png" alt="">
                    </div>
                </div>
                <div class="column has-text-centered">
                    <div class="title">关注公众号</div>
                    <div>
                        <img src="~/assets/footer/qr-pd.png" alt="">
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
      <aside class="menu is-mobile is-hidden-desktop">
        <p class="menu-label">智能门锁</p>
        <ul class="menu-list">
          <li>
            <a>M1</a>
          </li>
          <li>
            <a>P1</a>
          </li>
          <li>
            <a>T1</a>
          </li>
          <li>
            <a>H1</a>
          </li>
          <li>
            <a>配件</a>
          </li>
        </ul>
        <p class="menu-label">关于我们</p>
        <ul class="menu-list">
          <li>
            <a>公司简介</a>
          </li>
          <li>
            <a>品牌故事</a>
          </li>
          <li>
            <a>专利声明</a>
          </li>
          <li>
            <a>售后服务</a>
          </li>
        </ul>
        <p class="menu-label">品牌加盟</p>
        <ul class="menu-list">
          <li>
            <a>加盟</a>
          </li>
        </ul>
        <p class="menu-label">APP下载</p>
        <ul class="menu-list">
          <li>
            <a>加盟</a>
          </li>
        </ul>
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
.navbar-item {
  color: #888;
  font-size: 18px;
  margin-right: 55px;

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
    font-size:8px;
    color:rgba(0,0,0,1);
}
.footer p {color: #838383;}
.content {
    padding-bottom: 14px;
    border-bottom: 1px solid #DADADA;
}
.app-qr img{
    width:62px;
    height:62px;
    margin-right: 16px;
}
.copy .tel{
    font-size:15px;
    font-weight:500;
    color:rgba(106,106,106,1);
}
</style>

<script type="text/javascript">


export default {
  layout: "default",
  components: {},
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
