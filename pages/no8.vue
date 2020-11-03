<template>
  <div class="main-header">
    <div class="container">
      <a href="#" class="logo">
        <img src="@/assets/demo_logo.jpg" alt="" />
      </a>
      <div class="main-nav">
        <a href="#">金魚都能懂的系列</a>
        <a href="#">暴力網頁入門系列</a>
        <a href="#">CSS王可樂系列</a>
        <a href="#">RWD原來是醬子系列</a>
      </div>
    </div>
  </div>
</template>

<style scoped type="text/css">
.main-header {
  background: linear-gradient(0deg, #cc4380, #fb6c75);
}

.main-header .container {
  display: flex;
  padding: 20px;
  max-width: 1200px;
  justify-content: center;
  align-items: center;
  margin: auto;
}

.main-header .logo {
  width: 100px;
  position: absolute;
}

.main-header .logo img {
  width: 100%;
  vertical-align: middle;
}

.main-header .main-nav {
  margin: auto;
  display: flex;
}

.main-header .main-nav a:hover {
  transform: translateY(-5px);
}

.main-header .main-nav a {
  color: #fff;
  text-decoration: none;
  padding: 5px 1em;
  position: relative;
  transform: translateY(0px);
  transition: 0.3s;
}

.main-header .main-nav a:nth-child(3) {
  margin-left: 140px;
}
.main-header .main-nav a:after {
  content: "";
  position: absolute;
  height: 0;
  left: 50%;
  right: 50%;
  border-bottom: 1px solid #fff;
  bottom: -5px;
  transition: 0.3s;
}

.main-header .main-nav a:hover:after {
  left: 0;
  right: 0;
}
</style>