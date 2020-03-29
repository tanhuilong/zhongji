<template>
  <div class="about">
    <div class="container">
      <div class="header clearfloat">
            <div class="top-l clearfloat">
              <img src="../../public/img/menu_top_logo.png" >
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
      </div>
      <div class="content">
      <div class="aside left clearfloat">
        <helloworld></helloworld>
        <div class="nav">
        <router-link to="/"><el-button  size="mini" style="margin-top:6px">返回</el-button></router-link>
      <router-view></router-view>
      </div>
      </div>
      <div class="main">
   <zhu></zhu>
      </div>
      </div>
      </div>
  </div>
</template>
<script>
import helloworld from '../components/HelloWorld.vue' 
import zhu from '../components/Zhuyao.vue' 
export default {
  components:{
    helloworld,
    zhu
  }
}
</script>
<style lang="less">
.about{
  position:absolute;
  top:80px;
  left:-30px;
  .header{
  width:100%;
  height:50px;
  background:gray;
}
.content{
  display: flex;
}
.aside{
  width: 170px;
  height: 500px;
  background: purple;
}
.main{
  margin-left:20px;
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
 height: 40px;
 color:#fff;
}
.top-r li a{
  color:#fff;
}
.nav{
  margin-top: 350px;
  margin-left: 30px;
}
}
</style>