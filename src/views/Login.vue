<template>
<div>
  <el-form :model="loginForm"  label-width="100px" class="loginContainer">
    <h3 class="loginTitie">系统登录</h3>
    <el-form-item label="用户名" >
      <el-input type="text" v-model="loginForm.username" autocomplete="off" laceholder="请输入用户名"></el-input>
    </el-form-item>
    <el-form-item label="密码">
      <el-input type="password" v-model="loginForm.password" autocomplete="off" aria-placeholder="请输入密码"></el-input>
    </el-form-item>
    <el-form-item>
      <el-button type="primary" >提交</el-button>
      <el-button>重置</el-button>
    </el-form-item>
  </el-form>
</div>
</template>

<script>
export default {
  name: 'Login',
  data () {
    return {
      loginForm: {
        username: '',
        password: ''
      }
    }
  }
}
</script>

<style >
  .loginContainer{
    border-radius: 15px;
    background-clip: border-box;
    margin: 180px auto;
    width:350px;
    padding: 15px 35px 15px;
    background: aliceblue;
    border: 1px solid #161817;
    box-shadow: 0 0 25px #232625;
  }
  .loginTitie{
    margin: 20px auto 20px auto;
    text-align: center;
  }
</style>
