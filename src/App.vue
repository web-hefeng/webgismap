<template>
  <div id="app">
    <el-container class="app-out-panel">
      <el-header class="sys-header">系统标题</el-header>
      <el-container class="app-context-panel">
        <el-aside class="left-aside" width='200px'>左侧菜单</el-aside>
        <el-main class="sys-content">
          <Mapview />
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import Mapview from './components/common/Mapview';
export default {
  name: "App",
  components: {
    Mapview
  },
};
</script>

<style>
html,
body,
#app {
  position: relative;
  width: 100%;
  height: 100%;
  margin: 0;
}
.app-out-panel,.app-context-panel{
  height: 100%;
}
.sys-header{
  background-color: blue;
}
.left-aside{
  background-color:gray;
}
.sys-content {
  margin: 0;
  padding: 0;
}
</style>
