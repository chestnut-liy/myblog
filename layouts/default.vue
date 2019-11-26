<template>
  <div class="default-wrap">
    <top-nav></top-nav>
    <div class="default-container">
      <nuxt class="container-center" />
      <left-nav></left-nav>
      
      <right-nav></right-nav>
    </div>
  </div>
</template>
<script>
import leftNav from "~/components/leftNav.vue";
import topNav from "~/components/topNav.vue";
import rightNav from "~/components/rightNav.vue";
export default {
  components: {
    leftNav,
    topNav,
    rightNav
  }
};
</script>
<style  lang='scss' scoped>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
.default-wrap {
  .default-container {
    width: 100%;
    margin-top: 60px;
    overflow: hidden;
    /deep/ .left-nav-wrap {
      float: left;
      margin-left: -100%;
    }
    .container-center {
      float: left;
      width: 100%;
      height: 200px;
    }
    /deep/ .right-nav-wrap {
      float: left;
      margin-left: -300px;
    }
  }
}
</style>
