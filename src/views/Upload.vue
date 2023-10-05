<template>
  <div class="container">
    <div class="box1">
      <el-upload
          class="upload-demo"
          drag
          action="https://jsonplaceholder.typicode.com/posts/"
          multiple
          :file-list="fileList">
        <i class="el-icon-upload"></i>
        <div class="el-upload__text">Drag files here, or<em> Click to upload</em></div>
      </el-upload>
    </div>
    <div class="box2">
      <router-link to="/result">
        <el-button type="primary" class="button1">Run</el-button>
      </router-link>
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
    position: relative;
    left: 25px;
  }
  .box1,.box2{
    padding: 10px;
    //border: 1px solid #000;
    margin: 10px;
  }
</style>

<script>
export default {
  name: "Upload",
  data() {
    return {
      fileList: [{name: 'example', url: ''}]
    };
  }
}
</script>