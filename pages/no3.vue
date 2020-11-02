<template>
  <div class="wrap">
    <div class="item">
      <img src="https://picsum.photos/300/300/?random=1" />
      <div class="txt">
        <h2>CSS可樂</h2>
        <p>
          一個優質的技術型 Youtube
          頻道，旨在讓更多網路新手跳坑學習網站開發技術，平日用簡單易懂的方式讓新手能跨進網頁設計領域，並開設知名的網路課程「網頁設技暴力入門班」用紮實的原理讓新手能學習到深入的網頁製作技術及知識。
        </p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/300/?random=2" />
      <div class="txt">
        <h2>CSS可樂</h2>
        <p>
          一個優質的技術型 Youtube
          頻道，旨在讓更多網路新手跳坑學習網站開發技術，平日用簡單易懂的方式讓新手能跨進網頁設計領域，並開設知名的網路課程「網頁設技暴力入門班」用紮實的原理讓新手能學習到深入的網頁製作技術及知識。
        </p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/300/?random=3" />
      <div class="txt">
        <h2>CSS可樂</h2>
        <p>
          一個優質的技術型 Youtube
          頻道，旨在讓更多網路新手跳坑學習網站開發技術，平日用簡單易懂的方式讓新手能跨進網頁設計領域，並開設知名的網路課程「網頁設技暴力入門班」用紮實的原理讓新手能學習到深入的網頁製作技術及知識。
        </p>
      </div>
    </div>
  </div>
</template>

<style type="text/css">
* {
  padding: 0;
  margin: 0;
  list-style: none;
}

html,
body {
  height: 100%;
}

body {
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #003;
}

.wrap {
  width: 1200px;
  display: flex;
  margin: auto;
}

.item {
  width: 368px;
  margin: 15px;
  text-align: center;
  background-color: #fff;
  border: 1px solid #ccc;
  transform: translateY(0px);
  transition: 0.5s;
}

.item img {
  width: 100%;
  vertical-align: middle;
}

.item h2 {
  border-bottom: 1px solid #888;
  padding-bottom: 0.3em;
  margin-bottom: 0.3em;
  font-weight: 900;
  transition: .25s;
}

.item p {
  line-height: 1.6;
  transition: .25s;
}

.item .txt {
  padding: 20px;
  position: relative;
}

.item .txt::before {
  content: "";
  position: absolute;
  width: 0;
  height: 0;
  left: 0;
  top: 0;
  border-top: 50px solid transparent;
  border-left: 184px solid #fff;
  border-right: 184px solid #fff;
  transform: translateY(-100%);
}

.item:hover {
  transform: translateY(-25px);
}

.item:hover .txt {
  background: linear-gradient(0deg, #fb8076, #feb85d);
}

.item:hover .txt:before {
  border-left: 184px solid #feb85d;
  border-right: 184px solid #feb85d;
}
.item:hover h2 {
    color:#fff;
    border-bottom-color: #fff;
}
.item:hover p {
    color:#fff;
}
</style>