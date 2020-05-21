<template>
<div>
<el-tabs type="card" @tab-click="handleClick">
    <el-tab-pane label="User" to="/movie">User
        <el-form>
            <el-input type="textarea" :rows="2" placeholder="Please input" v-model="textarea">
            </el-input>
        </el-form>
    </el-tab-pane>
    <el-tab-pane label="Config">Config</el-tab-pane>
    <el-tab-pane label="Role">Role</el-tab-pane>
    <el-tab-pane label="Task">Task</el-tab-pane>
  </el-tabs>
</div>
</template>

<script>
export default {
  data () {
    return {
      textarea: ''
    }
  }
}
</script>

<style scoped>

</style>
