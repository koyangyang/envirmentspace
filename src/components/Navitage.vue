<template>
  <div id="navitage">
      <el-tabs v-model="activeName" @tab-click="handleClick">
    <el-tab-pane label="实验目的" name="first">
      <Content1/>
    </el-tab-pane>
    <el-tab-pane label="实验原理" name="second">
      <Content2/>
    </el-tab-pane>
    <el-tab-pane label="实验教学方法" name="third">
      <Content3/>
    </el-tab-pane>
    <el-tab-pane label="考核要求" name="fourth">
      <Content4/>
    </el-tab-pane>
    <el-tab-pane label="实验项目特色" name="fifth">
      <Content5/>
    </el-tab-pane>
    <el-tab-pane label="实验教学项目持续建设服务计划" name="sixth">
      <Content6/>
    </el-tab-pane>
  </el-tabs>
  </div>
</template>

<style scoped>
#navitage{
  padding-left: 30px;
  padding-right: 30px;
}

</style>
<script>
  import Content1 from '@/components/content/Content1'
  import Content2 from '@/components/content/Content2'
  import Content3 from '@/components/content/Content3'
  import Content4 from '@/components/content/Content4'
  import Content5 from '@/components/content/Content5'
  import Content6 from '@/components/content/Content6'
  export default {
    name:"Navigate",
    data() {
      return {
        activeName: 'first'
      };
    },
    methods: {
      handleClick(tab, event) {
        console.log(tab, event);
      }
    },
    components:{
      Content1,
      Content2,
      Content3,
      Content4,
      Content5,
      Content6
    }
  };
</script>
