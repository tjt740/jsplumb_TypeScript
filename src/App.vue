<template>
  <el-container class="wrap">

    <el-container class="my-app-container">
      <keep-alive>
        <router-view></router-view>
      </keep-alive>
    </el-container>
  </el-container>
</template>

<script>
export default {};
</script>
<style lang="scss">
html {
  height: 100%;
  body {
    margin: 0;
    padding: 0;
    height: 100%;
    overflow: hidden;
  }
  .wrap {
    height: 100%;

    .fy_el-header {
      background: #212528;
      color: #fff;
      z-index: 1000;
      font-size: 14px;
      line-height: 50px;
      padding-left: 5px;
      img {
        height: 36px;
        position: relative;
        top: 4px;
      }
      span.logoFont {
        font-size: 16px;
        margin-left: 20px;
        position: relative;
        top: -9px;
        margin-right: 100px;
      }
      .navItem {
        color: #fff;
        display: inline-block;
        height: 42px;
        line-height: 42px;
        padding: 0 20px;
        position: relative;
        top: -10px;
        text-decoration: none;
        &.active {
          background: hsla(0,0%,100%,.2);
        }
      }
      .el-dropdown{
        float: right;
        height: 42px;
        .el-dropdown-link{
          color: #fff;
        }

      }
    }

    .my-app-container{
      height: calc(100% - 42px);
    }
  }
}
::-webkit-scrollbar {
    width: 6px;
    height: 6px;
}
::-webkit-scrollbar-track {
    border-radius: 3px;
    background: rgba(0,0,0,0.06);
    box-shadow: inset 0 0 5px rgba(0,0,0,0.08);
}
/* 滚动条滑块 */
::-webkit-scrollbar-thumb {
    border-radius: 3px;
    background: rgba(0,0,0,0.12);
    box-shadow: inset 0 0 10px rgba(0,0,0,0.2);
}

</style>
