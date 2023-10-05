<template>
  <div class="container">
    <div class="box1">
      <router-link to="/trans">
        <el-button type="primary" class="button1">Back</el-button>
      </router-link>
    </div>
    <div class="box2">
      <el-descriptions direction="vertical" :column="1" border>
        <el-descriptions-item label="Model Name">wav2vec2</el-descriptions-item>
        <el-descriptions-item label="Model Discription">XXXXXXXXXXXX</el-descriptions-item>
        <el-descriptions-item label="Accuracy">70%</el-descriptions-item>
        <el-descriptions-item label="Deletion(DEL)">xxx</el-descriptions-item>
        <el-descriptions-item label="Insertions(INS)">xxx</el-descriptions-item>
        <el-descriptions-item label="Substitutions(SUB)">xxx</el-descriptions-item>
      </el-descriptions>
    </div>
  </div>
</template>
<style>
  .container{
    position: relative;
    display: flex;
    flex-direction: column;
  }
  .button1{
    position: absolute;
    top: 10px;
    right: 30px;
  }
  .box1,.box2{
    padding: 10px;
    //border: 1px solid #000;
    margin: 10px;
  }
</style>


<script>
export default {
  name: "Details"
}
</script>