<template>
  <div id="aside">
  <div class="demo">
    <div class="button2">
      <el-row>
         <el-button type="primary" @click="goPage('https://fileb6307dc47521.vrh5.cn/v3/idea/Bc7t4NuC')" plain>
          仿真实验
        </el-button>
      </el-row>
    </div>

    <div class="span"><span><el-link disabled>手机扫描下方二维码开始实验</el-link></span></div>
      <div class="block">
        <el-image :src="circleUrl"></el-image>
      </div>
    </div>
    <div class="font">
      <p><i class="el-icon-box"></i>&nbsp;项目</P>环境空间
      <p><i class="el-icon-school"></i>&nbsp;学校</p>河南科技大学
    </div>
  </div>
</template>

<style scoped>
/* .block{
  margin-top: -40px;
}
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
  } */





</style>

<script>
  export default {
   data () {
      return {


        circleUrl: "../../static/img/3.png",


      }
    },
    name:"Aside",
    methods:{
      goPage:function(url){
        window.location.href = url;
    }
    }
  };
</script>
