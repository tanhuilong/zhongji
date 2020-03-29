<template>
    <div class="home">
        <div class="mid ">
            <el-row :gutter="10">
             <el-col :span="6" :offset="1"><div class="grid-content bg-purple">
                     角色类型：<el-input
                placeholder="全部"
                suffix-icon="el-icon-d-caret"
                v-model="input1">
                </el-input>
                </div></el-col>
             <el-col :span="6"><div class="grid-content bg-purple">用户姓名：<el-input
                    placeholder="不选择"
                    suffix-icon="el-icon-d-caret"
                    v-model="input2">
                 </el-input>
                 </div></el-col>
             <el-col :span="2"><div class="grid-content bg-purple"><el-button type="danger" size="mini" style="margin-top:6px" >搜索</el-button></div></el-col>
             <el-col :span="2"><div class="grid-content bg-purple"><el-button  size="mini" style="margin-top:6px">重置</el-button></div></el-col>
             <el-col :span="2" :offset="3"><div class="grid-content bg-purple"><el-button type="danger" size="mini" style="margin-top:6px">新增角色</el-button></div></el-col>
           </el-row>
        </div>
        <div class="z-main"></div>
    </div>
</template>
<script>

export default {
   
    data(){
        return{
            input1:'',
            input2:''
        }
    }
}
</script>
<style lang="less">
.home{
  position:absolute;
  top:-390px;
  left: 190px;
  z-index: 10;

.mid{
    height: 80px;
    width:100%;
    background:#f5efef;
}
.el-col div ul li{
    float:left;
}
.el-col div{
    color:gray;
    font-size: 10px;
}
}
</style>
