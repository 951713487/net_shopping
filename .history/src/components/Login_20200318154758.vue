<template>
  <div class="background">
    <div id="login_box">
      <h1>Login</h1>
      <div class="form" :rules="loginFormRule">
        <div class="item">
          <i class="el-icon-user-solid"></i>
          <input placeholder="Username" prefix-icon="el-icon-search" type="text" :model="username" />
        </div>
        <div class="item">
          <i class="el-icon-lock"></i>
          <input
            placeholder="Password"
            prefix-icon="el-icon-search"
            type="password"
            :model="password"
          />
        </div>
      </div>
      <el-button type="info" round @click="signin">Login</el-button>
    </div>
  </div>
</template> 

<script>
export default {
  data() {
    return {
      form: {
        username: "ddd",
        password: "dadfadfad "
      },
      loginFormRule: {
        username: [
          { required: true, message: "请输入用户名", trigger: "blur" },
          { min: 3, max: 5, message: "长度在 3 到 5 个字符", trigger: "blur" }
        ],
        password: [
          { required: true, message: "请输入密码", trigger: "blur" },
          { min: 6, max: 12, message: "长度在 6 到 12 个字符", trigger: "blur" }
        ]
      }
    };
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
  background: #ffffff00; // 透明色
  color: #000000;
}

#login_box button {
  margin-top: 15px;
  width: 200px;
  height: 30px center;
}
.background {
  background: url(../img/bgimg.jpg);
  background-repeat: no-repeat center;
  background-size: 100% auto;
  position: fixed;
  height: 100%;
  width: 100%;
}
</style>