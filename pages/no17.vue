<template>
  <div class="wrap">
    <div class="login">
      <form action="#">
        <h2>會員登入</h2>
        <div class="group">
          <label for="userid">帳號</label>
          <input type="text" id="userid" />
        </div>
        <div class="group">
          <label for="password">密碼</label>
          <input type="password" id="password" />
        </div>
        <div class="btn-group">
          <button class="btn">登入</button>
          <button class="btn">取消</button>
        </div>
      </form>
    </div>
  </div>
</template>

<style type="text/css">
html,
body {
  height: 100%;
}
.wrap {
  background: url("https://picsum.photos/1200/900/?random=100") no-repeat center
    center/cover;
  display: flex;
  height: 100%;
  width: 100%;
  justify-content: center;
  align-items: center;
}
.login {
  height: 500px;
  width: 600px;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 10px;
  border: 10px solid #fff;
  box-shadow: 0 0 60px #000;
  backdrop-filter: blur(5px);
  display: flex;
  justify-content: center;
  align-items: center;
}
form {
  width: 400px;
  color: #fff;
}
form h2 {
  margin-bottom: 20px;
  padding-bottom: 20px;
  border-bottom: 1px solid #fff;
}
form .group {
  margin-bottom: 20px;
}
form label {
  line-height: 2;
}
form input {
  width: 100%;
  border: 1px solid #aaa;
  line-height: 3;
  border-radius: 5px;
}
form .btn-group {
  font-size: 0;
  margin-top: 50px;
}
form .btn {
  font-size: 20px;
  border: none;
  background-color: #6ab4fe;
  border-radius: 5px;
  width: 190px;
  padding: 10px 0px;
  color: #fff;
}
form .btn + .btn {
  margin-left: 20px;
}
</style>