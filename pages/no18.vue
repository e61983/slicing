<template>
  <div class="wrap">
    <div class="dialgure">
      <div class="user remote">
        <div class="avatar">
          <div class="pic">
            <img
              src="https://randomuser.me/api/portraits/med/men/27.jpg"
              alt="remote user"
            />
          </div>
          <div class="name">Tom</div>
        </div>
        <div class="txt">安安</div>
      </div>
      <div class="user local">
        <div class="avatar">
          <div class="pic">
            <img
              src="https://randomuser.me/api/portraits/med/women/17.jpg"
              alt="local user"
            />
          </div>
          <div class="name">Cady</div>
        </div>
        <div class="txt">?</div>
      </div>
    </div>
  </div>
</template>

<style scoped type="text/css">
.wrap {
  height: 100%;
  display: flex;
  align-items: center;
  padding: 10px;
}
.dialgure {
  width: 500px;
  padding: 20px;
  box-shadow: 0 0 10px #3e92cc;
  background-color: #f4f5f7;
  border-radius: 5px;
}
.user {
  display: flex;
  margin-bottom: 20px;
  align-items: flex-start;
}
.user .avatar {
  width: 60px;
  text-align: center;
  flex-shrink: 0;
}
.remote .name {
  color: #aaa;
}
.user .pic {
  border-radius: 50%;
  overflow: hidden;
}
.user .pic img {
  width: 100%;
  vertical-align: middle;
}
.user .txt {
  background-color: #ccc;
  padding: 16px;
  border-radius: 10px;
  position: relative;
  box-shadow: 5px 5px 10px #e4e5e7;
}
.remote .txt {
  margin-left: 20px;
  margin-right: 80px;
  background-color: #fff;
  color: #a1bec5;
}
.local {
  justify-content: flex-end;
}
.local .txt {
  margin-right: 20px;
  margin-left: 80px;
  order: -1;
  background-color: #3e92cc;
  color: #fff;
}
.local .txt::before,
.remote .txt::before {
  content: "";
  position: absolute;
  top: 20px;
  border-top: 10px solid transparent;
  border-bottom: 10px solid transparent;
}
.remote .txt::before {
  border-right: 10px solid #fff;
  left: -10px;
}
.local .txt::before {
  border-left: 10px solid #3e92cc;
  right: -10px;
}
</style>