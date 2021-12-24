<template>
  <div id="aside">
  <div class="demo">
    <div class="button2">
      <el-row>  
         <el-button type="primary" plain>
          <el-link href="https://fileb6307dc47521.vrh5.cn/v3/idea/Bc7t4NuC" target="_blank">
            仿真实验
          </el-link>
          </el-button>
      </el-row>
    </div>
    <div class="span"><span>实验二维码</span></div>
    <div class="block">
      <el-image :src="circleUrl"></el-image>
    </div>
  </div>
  <div class="font">
 
    <el-descriptions class="margin-top" column="1" direction="vertical">

    <el-descriptions-item label="项目">环境空间</el-descriptions-item>

    <el-descriptions-item label="学习">河南科技大学</el-descriptions-item>
    </el-descriptions>

    
    </div>


  </div>
</template>

<style scoped>
 .button2{
 
  position: absolute;
  right: 17%;
  top:-40px;
}
.span{
 
  margin-right:1px;
}
  #aside{
    padding-left: 30px;
  }
  .demo{
  height:340px;
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
