<template>
  <div class="background">
    <div id="login_box">
      <h1>Login</h1>
      <div class="form">
        <div class="item">
          <i class="el-icon-user-solid"></i>
          <input placeholder="Username" prefix-icon="el-icon-search" type="text" />
        </div>
        <div class="item">
          <i class="el-icon-lock"></i>
          <input placeholder="Password" prefix-icon="el-icon-search" type="password" />
        </div>
      </div>
      <el-button type="info" round>Login</el-button>
    </div>
  </div>
</template> 

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style lang="less" scoped>
#login_box {
  width: 30%;
  height: auto;
  border: 1px #000;
  margin: 0 auto;
  margin-top: 15%;
  text-align: center;
  background-color: #00000060;
  padding: 20px 50px;
}

#login_box .form {
  margin-top: 50px;
}
#login_box .form .item {
  margin-top: 15px;
}
#login_box .form .item i {
  font-size: 18px;
  color: #fff;
}
#login_box .form .item input {
  width: 180px;
  font-size: 18px;
  border: 0;
  border-bottom: 2px solid #fff;
  padding: 5px 10px;
  background: #ffffff00;
  color: #fff;
}

#login_box button {
  margin-top: 15px;
  width: 200px;
  height: 30px center;
}
.background{
    background-image: url(../img/background.jpg);
}
</style>