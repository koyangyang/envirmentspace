<template>
  <el-container>
    <el-header height="400px">
      <div class="video">
        <video controls="controls" width="400px" height="200px">
          <source src="../../static/video/1.mp4" type="video/mp4" />
        </video>
      </div>
      <div class="button">
        <el-row>
          <el-button type="primary" @click="goPage('https://fileb6307dc47521.vrh5.cn/v3/idea/Bc7t4NuC')">
            开始实验
          </el-button>
        </el-row>
      </div>
      <div class="title">
        <Title/>
      </div>
    </el-header>
    <el-main>
      <el-row :gutter="20">
        <el-col :span="3"><div class="grid-content bg-purple"></div></el-col>
        <el-col :span="14">
          <div class="grid-content bg-purple1">
              <Navigate/>
          </div></el-col>
        <el-col :span="4">
          <div class="grid-content bg-purple1">
            <Aside/>
          </div></el-col>
        <el-col :span="3"><div class="grid-content bg-purple"></div></el-col>
      </el-row>
    </el-main>
  </el-container>
</template>

<script>
import Navigate from '@/components/Navitage'
import Aside from '@/components/Aside'
import Title from '@/components/Title'
export default {
  name: "Body",
  components:{
    Navigate,
    Aside,
    Title
  },
  methods:{
    goPage:function(url){
        window.location.href = url;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.button{
  position: absolute;
  left: 10%;
  top:40%;
}
.video{
  position: absolute;
  right: 10%;
  top:50px;
}
.el-header {
  background: url("../../static/img/1.png");
  color: #333;
  text-align: center;
}
.el-main {
  background-color: #f4f4f4;
  color: #333;
  text-align: center;
  /* line-height: 160px; */
}

body > .el-container {
  margin-bottom: 40px;
}


/* .el-row {
  margin-bottom: 20px;
  &:last-child {
    margin-bottom: 0;
  }
} */
.el-col {
  border-radius: 4px;
}
.bg-purple {
  background: #f4f4f4;
}
.bg-purple1 {
  background: white;
}
.grid-content {
  border-radius: 4px;
  min-height: 36px;
}
</style>
