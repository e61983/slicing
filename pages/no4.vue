<template>
  <div class="wrap">
    <div class="item">
      <div class="pic">
        <img src="https://picsum.photos/600/350/?random=1" />
      </div>
      <div class="txt">
        <h2>金魚都懂的切版</h2>
        <p>敲碗敲了好久好久終於....碗破了，金魚就跑出來啦。</p>
      </div>
    </div>

    <div class="item">
      <div class="txt">
        <h2>我的記憶力只有七秒</h2>
        <p>敲碗敲了好久好久終於....碗破了，金魚就跑出來啦。</p>
      </div>
      <div class="pic">
        <img src="https://picsum.photos/600/350/?random=2" />
      </div>
    </div>

    <div class="item">
      <div class="pic">
        <img src="https://picsum.photos/600/350/?random=3" />
      </div>
      <div class="txt">
        <h2>金魚都懂的切版</h2>
        <p>敲碗敲了好久好久終於....碗破了，金魚就跑出來啦。</p>
      </div>
    </div>

    <div class="item">
      <div class="txt">
        <h2>我的記憶力只有七秒</h2>
        <p>敲碗敲了好久好久終於....碗破了，金魚就跑出來啦。</p>
      </div>
      <div class="pic">
        <img src="https://picsum.photos/600/350/?random=4" />
      </div>
    </div>
  </div>
</template>

<style type="text/css">
* {
  margin: 0;
  padding: 0;
  list-style: none;
}

body {
  padding: 100px 0;
  background: linear-gradient(20deg, #3d549c, #1aa2a0) fixed center center /
    100% 100%;
}

.wrap {
  width: 1200px;
  margin: auto;
}
.item {
  display: flex;
  align-items: center;
  margin: 70px;
}
.item .pic {
  width: 55%;
  flex-shrink: 0;
}
.item .pic img {
  width: 100%;
  vertical-align: middle;
}
.item .txt {
  width: 55%;
  flex-shrink: 0;
  padding: 50px 30px;
  box-sizing: border-box;
  position: relative;
  z-index: 1;
}

.item > :first-child {
  margin-right: -10%;
}

.item:nth-child(1) .txt {
  background-color: rgba(240, 174, 193, 0.8);
}
.item:nth-child(2) .txt {
  background-color: rgba(42, 253, 208, 0.8);
}
.item:nth-child(3) .txt {
  background-color: rgba(254, 201, 121, 0.8);
}
.item:nth-child(4) .txt {
  background-color: rgba(149, 219, 214, 0.8);
}
</style>