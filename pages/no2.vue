<template>
  <div class="wrap">
    <div class="item">
      <img src="https://picsum.photos/500/400/?random=5" />
      <div class="txt">
        <h2>金魚都能懂的這個網頁畫面怎麼切 : 互動圖文卡片</h2>
        <p>
          互動圖文卡片是我們在網頁中經常見到的另一種稀飯版，不會切你就遜掉囉。
        </p>
      </div>
    </div>

    <div class="item">
      <img src="https://picsum.photos/500/400/?random=10" />
      <div class="txt">
        <h2>金魚都能懂的這個網頁畫面怎麼切 : 互動圖文卡片</h2>
        <p>
          互動圖文卡片是我們在網頁中經常見到的另一種稀飯版，不會切你就遜掉囉。
        </p>
      </div>
    </div>

    <div class="item">
      <img src="https://picsum.photos/500/400/?random=20" />
      <div class="txt">
        <h2>金魚都能懂的這個網頁畫面怎麼切 : 互動圖文卡片</h2>
        <p>
          互動圖文卡片是我們在網頁中經常見到的另一種稀飯版，不會切你就遜掉囉。
        </p>
      </div>
    </div>

    <div class="item">
      <img src="https://picsum.photos/500/400/?random=30" />
      <div class="txt">
        <h2>金魚都能懂的這個網頁畫面怎麼切 : 互動圖文卡片</h2>
        <p>
          互動圖文卡片是我們在網頁中經常見到的另一種稀飯版，不會切你就遜掉囉。
        </p>
      </div>
    </div>
  </div>
</template>

<style type="text/css" scoped>

.wrap {
  width: 100%;
  display: flex;
}
.item {
  width: 25%;
  position: relative;
}
.item img {
  width: 100%;
  vertical-align: middle;
}

.item .txt {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 20px;
  background-color: rgba(0, 0, 0, 0.6);
  display: flex;
  justify-content: center;
  flex-direction: column;
  opacity: 0;
  transition: opacity 0.6s;
}

.item:hover .txt {
  opacity: 1;
}

.item .txt h2 {
  font-size: 28px;
  color: #ff0;
  font-weight: 500;
}

.item .txt h2:after {
  content: "";
  display: block;
  width: 0%;
  height: 1px;
  margin: 10px, 0;
  background-color: #ff0;
  transition: width 0.5s 0.5s;
}

.item:hover h2:after {
  width: 100%;
}

.item .txt p {
  font-size: 18px;
  color: #fff;
  font-weight: 100;
}
</style>