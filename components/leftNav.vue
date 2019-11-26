<template>
  <div class="left-nav-wrap">
    <ul>
      <li v-for="(item,index) in navList" :key="index">
        <nuxt-link :to="item.router">
          <svg class="icon" aria-hidden="true">
            <use :xlink:href="[item.icon]" />
          </svg>
          <!-- <i :class = "['iconfont', item.icon]"></i> -->
          {{item.name}}
        </nuxt-link>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      navList: [
        {
          name: "明殿",
          icon: "#iconzhiwu",
          router: "/"
        },
        {
          name: "宁静寺",
          icon: "#iconzhongqiujie",
          router: "/article/article"
        },
        {
          name: "无色庵",
          icon: "#iconyuanxiaojie",
          router: ""
        },
        {
          name: "丹室",
          icon: "#icondiqiuyi",
          router: ""
        },
        {
          name: "粉巷",
          icon: "#iconpinganye",
          router: ""
        },
        {
          name: "天涯",
          icon: "#iconertongjie",
          router: ""
        },
        {
          name: "狂浪生",
          icon: "#iconwanshengjie",
          router: ""
        },
        {
          name: "得道",
          icon: "#iconsushi",
          router: ""
        },
        {
          name: "百鸣苑",
          icon: "#iconningmeng",
          router: ""
        }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
@import "../assets/scss/app.scss";
.left-nav-wrap {
  width: 200px;
  // background-color: $background-color;
  ul {
    text-align: left;
    li {
      line-height: 60px;
      list-style: none;
      a {
        font-weight: 700;
        color: $theme-color;
        &:hover {
          color: $opcity-color;
        }
      }
      &:hover {
        color: $opcity-color;
        background-color: $background-color;
        // border-radius: 30px;
      }
    }
  }
}
</style>