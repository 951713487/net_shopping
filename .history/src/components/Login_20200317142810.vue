<template>
  <div id="login_box">
    <h2>Login</h2>
    <div>
      <input placeholder="username" prefix-icon="el-icon-search" v-model="input1" type="text" />
    </div>
    <div>
      <input placeholder="password" prefix-icon="el-icon-search" v-model="input2" type="password" />
    </div>
    <el-button type="info" round>Login</el-button>
  </div>
</template> 

<script>
export default {};
</script>

<style lang="less" scoped>
#login_box {
    width:30%;  
    height:300px;
    border:1px solid #000;
    margin: 0 auto;
    margin: 15%;
}


</style>