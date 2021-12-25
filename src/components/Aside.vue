<template>
<div id="aside">
    <div class="button">
      <el-row>
        <el-button type="primary" @click="goPage('https://fileb6307dc47521.vrh5.cn/v3/idea/Bc7t4NuC')" plain>仿真实验</el-button>
      </el-row>
    </div>
    <div class="span"><span><el-link type="warning" disabled>手机扫描下方二维码开始实验</el-link></span>
      <div class="block">
        <el-image :src="circleUrl"></el-image>
      </div>
    </div>
    <div class="font">
      <p><i class="el-icon-box"></i>&nbsp;项目</P>环境空间实验
      <p><i class="el-icon-school"></i>&nbsp;学校</p>河南科技大学
    </div>
</div>
</template>

<style scoped>
  #aside{
    padding-top: 20px;
    line-height: 40px;
  }
</style>

<script>
  export default {
   data () {
      return {
        circleUrl: "../../static/img/3.png",
        srcList: [
          '../../static/img/3.png'
        ]
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
