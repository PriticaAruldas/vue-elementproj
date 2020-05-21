<template>
  <el-form :model="form" :rules="rules" ref="ruleForm">
    <el-form-item label="Title" prop="title">
      <el-input v-model="form.title"></el-input>
    </el-form-item>
<el-form-item label="Release Date" prop="date">
      <el-date-picker v-model="form.date" type="date" placeholder="Release Date"></el-date-picker>
    </el-form-item>
<el-form-item label="Summary" prop="summary">
      <el-input v-model="form.summary" type="textarea"></el-input>
    </el-form-item>
<el-form-item>
      <input type="file" style="display: none" ref="file" @change="onChangeFileUpload($event)" />
      <el-button type="primary" @click="$refs.file.click()">Upload Photo</el-button>
    </el-form-item>
<el-form-item prop="photo">
      <img ref="photo" :src="form.photo" class="photo" />
    </el-form-item>
<el-form-item>
      <el-button type="primary" @click="submitForm('ruleForm')">Save</el-button>
    </el-form-item>
  </el-form>
</template>

<script>
export default {
}
</script>

<style scoped>

</style>
