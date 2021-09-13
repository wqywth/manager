<template>
  <div class="login">
    <el-form class="loginForm" label-position="top" label-width="80px" :model="formData">
      <h2>用户登录</h2>
      <el-form-item label="用户名">
        <el-input v-model="formData.username"></el-input>
      </el-form-item>
      <el-form-item label="密码">
        <el-input v-model="formData.password"></el-input>
      </el-form-item>
      <el-button class="loginbtn" type="primary">登录</el-button>
    </el-form>
  </div>
</template>

<script>
export default {
  name:'Login',
  data(){
    return{
      formData:{
        username:"",
        password:"",
      }
    }
      
  }
}
</script>

<style lang="less" scoped>
.login{
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  .loginForm{
  width: 460px;
  height: 400px;
  background-color: azure;
  padding: 0 20px;
  h2{
  
    text-align: center;
  }
  .loginbtn{
    width: 100%;
  }
}
}


</style> 