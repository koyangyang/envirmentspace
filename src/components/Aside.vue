<template>
  <div id="aside">
    <el-descriptions class="margin-top" title="简介" :column="1" direction="vertical">
    <el-descriptions-item label="项目">环境空间</el-descriptions-item>
    <el-descriptions-item label="学习">河南科技大学</el-descriptions-item>
    </el-descriptions>
    <el-row class="demo-avatar demo-basic">
      <el-col :span="10">
        <div class="sub-title">
            二维码
        </div>
        <div class="demo-basic--circle">
          <div class="block"><el-avatar shape="square" :size="100" :src="circleUrl">
            </el-avatar>
          </div>       
        </div>
      </el-col>   
    </el-row>


  </div>
</template>

<style scoped>
  #aside{
    padding-left: 30px;
  }
</style>

<script>
  export default {
   data () {
      return {
    
       
        circleUrl: "../../static/img/3.png",
        
        
      }
    },
    name:"Aside"
  };
</script>
