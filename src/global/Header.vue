<template>
  <div class="g-header">
    <!--<div class = "g-logo">-->
      <!--<img src="../assets/logo.png" alt="logo" />-->
    <!--</div>-->
    <div class="g-nav">
      <el-menu :default-active="activeIndex" mode="horizontal"
               class="i-nav" @select="handleSelect">
        <el-menu-item index="1">主页</el-menu-item>
        <el-submenu index="2">
          <template slot="title">我的工作台</template>
          <el-menu-item index="2-1">选项1</el-menu-item>
          <el-menu-item index="2-2">选项2</el-menu-item>
          <el-menu-item index="2-3">选项3</el-menu-item>
        </el-submenu>
      </el-menu>
    </div>
  </div>
</template>

<script>
  export default{
    name:'GlobalHeader',
      data(){

    },
    methods:{
      handleSelect (key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }

</script>

<style lang="scss">

</style>
