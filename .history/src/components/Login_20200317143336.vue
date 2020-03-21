<template>
  <div id="login_box">
    <h1>Login</h1>
    <div class="form">
      <div class="item">
        <i></i>
        <input placeholder="username" prefix-icon="el-icon-search" v-model="input1" type="text" />
      </div>
      <div class="item">
        <i></i>
        <input placeholder="password" prefix-icon="el-icon-search" v-model="input2" type="password" />
      </div>
    </div>
    <el-button type="info" round>Login</el-button>
  </div>
</template> 

<script>
export default {};
</script>

<style lang="less" scoped>
#login_box {
  width: 30%;
  height: 300px;
  border: 1px solid #000;
  margin: 0 auto;
  margin-top: 15%;
  text-align: center;
}

#login_box .form{
    margin-top:50px;

}

#login_box .form .item input{
    border: 0;
    border-bottom: 2px solid #000;
}
</style>