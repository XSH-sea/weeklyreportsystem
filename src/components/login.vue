<template>
  <div class="login-page">
      <el-form class="container" label-width="60px" label-position="right">
          <h3>用户登陆</h3>
          <el-form-item label="用户名:" >
            <el-input placeholder="请输入用户名"></el-input>
          </el-form-item>
          <el-form-item label="密码:">
            <el-input placeholder="请输入密码"></el-input>  
          </el-form-item>
              <el-button type="primary" icon="el-icon-user" @click="goIndex">登陆</el-button>
      </el-form>
  </div>
</template>

<script>
export default {
  data(){
    return{

    }
  },
  methods:{
    goIndex(){
      this.$router.push({
        path:"/index"
      })
    }
  }
}
</script>

<style>
.login-page{
    width: 100%;
    height: 100%;
}

.container{
    width: 350px;
    height: 250px;
    padding: 5px 10px 5px 10px; 
    border: 1px solid #eee;
    border-radius: 4px;
    box-shadow: 0 0 8px #ccc;
    margin: 200px auto;
}
</style>