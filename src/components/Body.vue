<template>
  <el-container>
    <el-header height="400px">
      <div id="detial">
          <Title/>
      </div>
      <div id="video">
        <video controls="controls" style="height:240px">
          <source src="../../static/video/1.mp4" type="video/mp4" />
        </video>
      </div>
    </el-header>
    <el-main>
      <el-row :gutter="20">
        <el-col :span="2"><div class="grid-content bg-purple"></div></el-col>
        <el-col :span="15">
          <div class="grid-content bg-purple1">
              <Navigate/>
          </div></el-col>
        <el-col :span="5">
          <div class="grid-content bg-purple1">
            <Aside/>
          </div></el-col>
        <el-col :span="2"><div class="grid-content bg-purple"></div></el-col>
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
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
#detial{
  flex: 1;
}
#video{
  flex: 1;
  text-align: center;
  padding-top: 60px;
  padding-left: 5%;
}
.el-header {
  background: url("../../static/img/1.png");
  display: flex;
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

/*手机*/
        /* @media screen and (max-width:600px){
           #video{
             display: none;
           }
           .el-header {
              background: url("../../static/img/1.png");
              display: inline;
              color: #333;
              text-align: center;
            }
            #detial{
              width: 100%;
            }
        } */
</style>
