<template>
  <div class="top-nav-wrap">
    <div class="top-nav-title">
      <h4>热爱生活。活在当下。</h4>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "../assets/scss/app.scss";
.top-nav-wrap {
  width: 100%;
  background-color: $light-background;
  position: fixed;
  top: 0;
  .top-nav-title {
      margin-left: 80px;
      text-align: left;
    h4 {
      color: $light-font-color;
    }
  }
}
</style>