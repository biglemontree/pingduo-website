<template>
  <div>
      <div class="top-link bg-f2 is-hidden-mobile">
          <div class="content flex justify-between">
              
                <nuxt-link to="/aboutus/company-produce" class=" has-text-centered">
                    <img src="~/assets/aboutus/icon_gsjj.png" alt="">
                    <div>
                        公司简介
                    </div>
                </nuxt-link>
                <nuxt-link to="/aboutus/brand-history" class="link has-text-centered">
                    <img src="~/assets/aboutus/icon_ppgs.png" alt="">
                    <div>
                        品牌故事
                    </div>
                </nuxt-link>
                <nuxt-link to="/aboutus/pd-only" class="link has-text-centered">
                    <img src="~/assets/aboutus/icon_zlsm.png" alt="">
                    <div>
                        专利声明
                    </div>
                </nuxt-link>
                <nuxt-link to="/aboutus/service" class="link has-text-centered">
                    <img src="~/assets/aboutus/icon_shfw.png" alt="">
                    <div>
                        售后服务
                    </div>
                </nuxt-link>
          </div>
      </div>
      <nuxt-child/>
  </div>
</template>

<script>
export default {
    data() {
        return {
            currentPath: '/aboutus/company-produce'
        }
    },
    created() {
        console.log(this)
        
    }
}
</script>

<style lang="less" scoped>
.top-link {
    height: 117px;
    .content {
        width: 546px;
        margin: 0 auto;
        height: 100%;
        padding: 33px 0 15px;
    }
}
</style>

