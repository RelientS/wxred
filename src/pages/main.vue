<template>
  <div class="container">
    <Header></Header>
    <div class="mainContainer">
        <el-row>
            <el-col :span="3" class="left-content">
              <el-menu
                default-active="2"
                class="el-menu-mymenu"
                >
                <el-submenu index="1">
                  <template slot="title">
                    <i class="el-icon-location"></i>
                    <span>发送</span>
                  </template>
                  <el-menu-item-group>
                    <el-menu-item index="1-1">Send Transation</el-menu-item>
                    <el-menu-item index="1-2">离线发送</el-menu-item>
                  </el-menu-item-group>
                </el-submenu>
                <el-menu-item index="2">
                  <i class="el-icon-menu"></i>
                  <span slot="title">货币交换</span>
                </el-menu-item>
                <el-menu-item index="3">
                  <i class="el-icon-document"></i>
                  <span slot="title">去中心化应用</span>
                </el-menu-item>
                <el-submenu index="4">
                  <template slot="title">
                    <i class="el-icon-phone-outline"></i>
                    <span>合约</span>
                  </template>
                  <el-menu-item-group>
                    <el-menu-item index="4-1">母鸡哇</el-menu-item>
                    <el-menu-item index="4-2">母鸡哇</el-menu-item>
                  </el-menu-item-group>
                </el-submenu>
                <el-submenu index="5">
                  <template slot="title">
                    <i class="el-icon-bell"></i>
                    <span>消息</span>
                  </template>
                  <el-menu-item-group>
                    <el-menu-item index="5-1">母鸡哇</el-menu-item>
                    <el-menu-item index="5-2">母鸡哇</el-menu-item>
                  </el-menu-item-group>
                </el-submenu>
              </el-menu>
            </el-col>
            <el-col :span="21" class="right-content">
              <el-row :gutter="10">
                  <el-col :span="8" ><div class="right-grid-content bg-purple-dark">这是右侧边栏</div></el-col>
                  <el-col :span="8" ><div class="right-grid-content bg-purple-dark">这是右侧边栏</div></el-col>
                  <el-col :span="8" ><div class="right-grid-content bg-purple-dark">这是右侧边栏</div></el-col>
              </el-row>
              <el-row :gutter="10">
                  <el-col :span="16" ><div class="right-main-content bg-purple-dark">这是右侧主容器</div></el-col>
                  <el-col :span="8" >
                    <div class="right-grid-content bg-purple-dark">这是右侧边栏</div>
                    <div class="last-grid-content right-grid-content bg-purple-dark">这是右侧边栏</div>
                  </el-col>
              </el-row>
            </el-col>
        </el-row>
    </div>
  </div>
</template>

<script>
import Header from '@/components/Header'
export default {
  data( ){
    return {

    }
  },
  components: {
    Header
  },
  methods: {
  }
}
</script>

<style lang="scss" scoped>
.container{
    height: 960px;
    width: 100%;
    background: #f9f9f9;
    .mainContainer{
        padding-top:80px;
        height: 1000px;
        width:100%;
        background: #f9f9f9;
    }
}
.el-row {
    padding: 0;
    margin-bottom: 10px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .el-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-white {
    background: #ffffff;
    height: 960px;
  }
  .bg-purple {
    background: #d3dce6;
    height: 960px;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
  .left-content {
    position: fixed;
    height: 1000px;
    border-radius: 0;
    text-align: left;
  }
  .right-content {
    height:800px;
    margin-left: 12.5%;
    padding: 10px;
  }
  .right-grid-content {
    height:150px;
  }
  .last-grid-content {
    margin-top:10px;
  }
  .right-main-content {
    height:750px;
  }
  .el-menu-mymenu{
    height: 1000px;
  }

</style>
