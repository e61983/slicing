<template>
  <div class="wrap">
    <div class="banner"></div>
    <div class="sec">
      <div class="container">
        <div class="item">
          <h2>Title</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero
            voluptatibus amet voluptas! Sapiente culpa, aliquid eaque molestiae
            iure maxime nihil dignissimos quibusdam eveniet modi. Fuga dolor
            esse asperiores labore quos!
          </p>
        </div>
        <div class="item">
          <h2>Title</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero
            voluptatibus amet voluptas! Sapiente culpa, aliquid eaque molestiae
            iure maxime nihil dignissimos quibusdam eveniet modi. Fuga dolor
            esse asperiores labore quos!
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped type="text/css">
.wrap {
}
.banner {
  height: 700px;
  background: url("https://picsum.photos/1400/960/?random=1") no-repeat center
    top / cover;
}
.sec {
  position: relative;
}
.sec .container {
  width: 1200px;
  margin: auto;
  display: flex;
  padding: 100px 0;
  z-index: 2;
  position: relative;
}
.sec .item {
  width: 570px;
  margin: 0 15px;
}
.sec .item h2 {
  margin-bottom: 1.3em;
}
.sec .item p {
  line-height: 1.7;
  margin-bottom: 1.6em;
}
.sec::after {
  content: "";
  display: block;
  position: absolute;
  width: 200px;
  height: 200px;
  background-color: #fff;
  top: 0;
  left: 50%;
  transform: translateY(-50%);
  border-radius: 50%;
  box-shadow: 178px 0px 0px 30px #fff, 327px 34px 0px 20px #fff,
    480px 9px 0px 20px #fff, 690px 71px 0px 60px #fff, 880px 0px 0px 89px #fff,
    -70px 0px 0px 0px #fff, -227px 52px 0px 20px #fff, -380px 19px 0px 20px #fff,
    -590px 61px 0px 60px #fff, -780px 0px 0px 89px #fff,
    178px -20px 0px 30px rgba(0, 0, 0, 0.5),
    257px -33px 0px 0px rgba(0, 0, 0, 0.5),
    360px -9px 0px 20px rgba(0, 0, 0, 0.5),
    670px -51px 0px 60px rgba(0, 0, 0, 0.5),
    860px 0px 0px 89px rgba(0, 0, 0, 0.5), -70px 0px 0px 0px rgba(0, 0, 0, 0.5),
    -237px -12px 0px 10px rgba(0, 0, 0, 0.5),
    -390px 0px 0px 10px rgba(0, 0, 0, 0.5),
    -540px -12px 0px 30px rgba(0, 0, 0, 0.5);
}
.sec::before {
  content: "";
  position: absolute;
  width: 100%;
  height: 200px;
  background-color: #fff;
  z-index: 1;
  top: 0;
  left: 0;
}
</style>