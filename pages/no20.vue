<template>
  <div class="wrap">
    <ul>
      <li class="box">CSS</li>
      <li class="box">金魚</li>
      <li class="box">網頁</li>
      <li class="box">切版</li>
      <li class="box">入門</li>
      <li class="box">HTML</li>
      <li class="box">教學</li>
      <li class="box">RWD</li>
      <li class="box">Bootstrap</li>
    </ul>
  </div>
</template>
<style scoped type="text/css">
.wrap {
}
ul {
  width: 960px;
  margin: auto;
  padding: 100px 0;
  display: flex;
  flex-wrap: wrap;
}
li {
  width: 200px;
  height: 200px;
  margin: 0 60px -40px;
  text-align: center;
  line-height: 200px;
  position: relative;
  font-size: 30px;
}
li::before {
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  transform: rotate(45deg);
  z-index: -1;
  transition: 0.3s;
}
li:nth-child(n + 4) {
  left: 160px;
}
li:nth-child(n + 7) {
  left: 0;
}
.box:nth-child(1)::before {
  background-color: #3ed0cd;
}
.box:nth-child(2)::before {
  background-color: #b2e086;
}
.box:nth-child(3)::before {
  background-color: #ef8899;
}
.box:nth-child(4)::before {
  background-color: #fc7b51;
}
.box:nth-child(5)::before {
  background-color: #2fccf9;
}
.box:nth-child(6)::before {
  background-color: #5f539b;
}
.box:nth-child(7)::before {
  background-color: #fce928;
}
.box:nth-child(8)::before {
  background-color: #7cc85c;
}
.box:nth-child(9)::before {
  background-color: #ffa55e;
}
.box:hover {
  color: #eee;
}
.box:hover::before {
  background-color: #000;
}
</style>