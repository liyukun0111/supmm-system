<template>
  <div class="index">
    <el-container>
      <!-- 左边 -->
      <el-aside width="200px">
        <!-- 导航菜单 -->
          <Nav></Nav>
      </el-aside>
      <el-container>
        <el-header>
          <!-- 头 -->
          <Top></Top>
        </el-header>
        <el-main>
          <router-view />
        </el-main>
        <el-footer>
          <!-- 脚 -->
          <Bottom></Bottom>
        </el-footer>
      </el-container>
    </el-container>
  </div>
</template>
<script>
// 引入导航组件
import Nav from '@/components/Nav/Nav.vue'
// 引入头部组件
import Top from '@/components/Top/Top.vue'
// 引入尾部组件
import Bottom from '@/components/Bottom/Bottom.vue'

export default {
  // 注册组件
  components: {
    Nav,
    Top,
    Bottom
  }
};
</script>

<style lang="less">
.index {
  height: 100%;
  .el-container {
    height: 100%;
    // 左侧
    .el-aside {
      background-color: #d3dce6;
      color: #333;
      text-align: center;
      height: 100%;
    }
    //   中间
    .el-main {
      background-color: #e9eef3;
      color: #333;
      text-align: center;
      height: 100%;
    }
    //   头部 & 尾部
    .el-header,
    .el-footer {
      background-color: #b3c0d1;
      color: #2d3a4b;
      text-align: center;
      line-height: 60px;
    }
  }
}


</style>
