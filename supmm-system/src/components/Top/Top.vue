<template>
  <div class="top">
    <el-row :gutter="20">
      <el-col :span="12">
        <div class="title">
          <i class="el-icon-menu"></i>
          华联超市管理系统
        </div>
      </el-col>
      <el-col :span="12">
        <div class="top-right">
          <el-row>
            <el-col :span="18">
              欢迎您!
              <span class="username">{{ username }}</span>
            </el-col>
            <el-col :span="6">
              <div class="avatar">
                <img width="100%" height="100%" :src="avatarUrl" alt>
              </div>
            </el-col>
          </el-row>
        </div>
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {
    data () {
        return {
            username: '王麻子',
            avatarUrl: 'http://127.0.0.1:8080/avatar.jpg'
        }
    }
};
</script>
<style lang="less">
    .top {
        // background-color: red;
        border-bottom: 2px solid green;
        .title {
            text-align: left;
            font-size: 20px;
            font-weight: 900;
        }
        .top-right {
            color: #2d3a4b;
            text-align: right;
            .username {
               font-weight: 600;
            }
            .avatar {
                width: 52px;
                height: 52px;
                margin-top: 4px;
                margin-left: 30px;
                border-radius: 50%;
                img {
                    border-radius: 50%;
                }
            }
        }
    }
</style>
