<template>
  <div id="title">
      <p id="name"><strong>环境空间灯光设计虚拟仿真实验</strong></p>
      <p class="tag">所属专业类：艺术与设计类&nbsp;&nbsp;&nbsp;&nbsp;对应专业：环境设计</p>
      <p class="tag">学校：河南科技大学&nbsp;&nbsp;&nbsp;&nbsp;学院：艺术与设计学院</p>
      <p id="textcontent">《环境空间灯光设计虚拟仿真实验》是针对“环境空间模型构件知识及光环境的设计”而营造的虚拟互动平台，以“翻转课堂——虚拟仿真平台实验——模型实训操作与考核”为一体化的教学方式。学生可以基于PC端或手机移动端在虚拟仿真环境中进行交互式实验，以此来弥补实训环节中无法模拟设计出光环境等限制性问题，提高学生对光环境的现实模拟能力从而切实提升学习效果。</p>
      <el-button type="primary" @click="goPage('https://fileb6307dc47521.vrh5.cn/v3/idea/Bc7t4NuC')">开始实验</el-button>
  </div>
</template>

<style scoped>
.el-button--primary{
  margin-top: 10px;
}
#name{
  font-size: 25px;
}
#textcontent{
  line-height: 25px
}
.tag{
  font-size: 15px;
  margin: 10px;
  color: rgb(210, 211, 215);
}
#title{
  text-align: left;
  position: absolute;
  width: 40%;
  left: 10%;
  top: 5%;
  color: white;
}
</style>

<script>
  export default {
    name:"Title",
    methods:{
      goPage:function(url){
          window.location.href = url;
      }
    }
  };
</script>
