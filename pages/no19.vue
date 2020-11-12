<template>
  <div class="wrap">
    <h1>金魚也懂得這個網頁怎麼切</h1>
    <ul class="timeline">
      <li>
        <a href="">
          <h2>第一天</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
            voluptatum accusamus sunt est praesentium aut alias. Animi fugit
            temporibus non!
          </p>
        </a>
      </li>
      <li>
        <a href="">
          <h2>第二天</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
            voluptatum accusamus sunt est praesentium aut alias. Animi fugit
            temporibus non!
          </p>
        </a>
      </li>
      <li>
        <a href="">
          <h2>第三天</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
            voluptatum accusamus sunt est praesentium aut alias. Animi fugit
            temporibus non!
          </p>
        </a>
      </li>
      <li>
        <a href="">
          <h2>第四天</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
            voluptatum accusamus sunt est praesentium aut alias. Animi fugit
            temporibus non!
          </p>
        </a>
      </li>
      <li>
        <a href="">
          <h2>第五天</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
            voluptatum accusamus sunt est praesentium aut alias. Animi fugit
            temporibus non!
          </p>
        </a>
      </li>
      <li>
        <a href="">
          <h2>第六天</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
            voluptatum accusamus sunt est praesentium aut alias. Animi fugit
            temporibus non!
          </p>
        </a>
      </li>
      <li>
        <a href="">
          <h2>第七天</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
            voluptatum accusamus sunt est praesentium aut alias. Animi fugit
            temporibus non!
          </p>
        </a>
      </li>
    </ul>
  </div>
</template>

<style type="text/css">
body {
  background-color: #edece1;
}
.wrap {
  max-width: 960px;
  margin: auto;
}
.wrap::after {
  display: block;
  content: "";
  clear: both;
  width: 100%;
  height: 0;
}
.timeline {
  margin: 100px 0 200px;
}
.timeline a {
  text-decoration: none;
  background-color: #fff;
  border: 1px solid #aaa;
  display: block;
  box-sizing: border-box;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 3px 3px 5px #999;
}
.timeline a:hover {
  background-color: #6fa5f6;
}
.timeline a:hover h2,
.timeline a:hover p {
  color: #eee;
}
.timeline li {
  width: 50%;
  box-sizing: border-box;
  padding: 20px 0;
  position: relative;
}
.timeline li:nth-child(odd) {
  float: left;
  padding-right: 100px;
}
.timeline li:nth-child(even) {
  float: right;
  padding-left: 100px;
  transform: translateY(50%);
}
.timeline li::after {
  z-index: -1;
}
.timeline li:nth-child(odd)::after {
  content: "";
  position: absolute;
  width: 1px;
  height: 100%;
  background-color: #ccc;
  top: 0;
  right: 0;
}
.timeline li:last-child::after {
  height: 50%;
}
.timeline li::before {
  content: "";
  position: absolute;
  width: 20px;
  height: 20px;
  border-radius: 50%;
  background-color: #aaa;
  top: 0;
  bottom: 0;
  margin: auto;
}
.timeline li:nth-child(odd)::before {
  right: -10px;
  z-index: 2;
}
.timeline li:nth-child(even)::before {
  left: -10px;
}
.timeline h2 {
  color: #333;
  font-weight: 700;
  border-bottom: 1px solid #888;
}
.timeline h2::before {
  content: "";
  position: absolute;
  height: 1px;
  width: 100px;
  top: 0;
  bottom: 0;
  margin: auto;
  background-color: #aaa;
}
.timeline li:nth-child(odd) h2::before {
  right: 0;
}
.timeline li:nth-child(even) h2::before {
  left: 0;
}
.timeline p {
  font-weight: 100;
  color: #666;
}
</style>