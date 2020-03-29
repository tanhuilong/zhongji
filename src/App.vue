<template>
  <div class="app">
      <el-container>
  <el-header>
    <div class="top-l clearfloat">
              <img src="../public/img/menu_top_logo.png" >
              <span>中央会员管理系统</span>
            </div>
            <div class="top-r right clearfloat">
              <ul>
               <li><el-avatar icon="el-icon-user-solid"></el-avatar></li>
               <li><a href="#">你好！ xxx</a></li>
               <li>|</li>
               <li><a href="#">退出登录</a></li>
               </ul>
            </div>
  </el-header>
  <el-container>
    <el-aside width="200px"><helloworld></helloworld></el-aside>
    <el-main>
        <div :class="z-top" >业绩管理/业绩报表</div>
   <zhu></zhu>
    </el-main>
  </el-container>
</el-container>

  </div>
</template>
<script>
import helloworld from './components/HelloWorld.vue' 
import zhu from './components/Zhuyao.vue' 
export default {
  components:{
    helloworld,
    zhu
  }
}
</script>
<style lang="less">
.app{
.el-header{
  width:100%;
  height:50px;
  background:gray;
}
.content{
  display: flex;
}
.el-aside{
  width: 170px;
  background: #545c64;
  position: relative;
}
.el-main{
  flex:1;
  height:500px;
}
.top-l img{
  margin: 10px;
}
.top-l{
  display: flex;
}
.top-l span{
  color:white;
  height: 50px;
  line-height: 50px;
}
.top-r{
  margin-top:-45px ;
}
.top-r ul{
list-style: none;
}
.top-r li{
 float:left;
 padding-right:5px ;
 line-height: 40px;
 color:#fff;
}
.top-r li a{
  color:#fff;
}
.z-top{
    height :30px;
    background :white;
    color:gray;
}
}
</style>
