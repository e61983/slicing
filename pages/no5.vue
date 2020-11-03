<template>
  <div class="wrap">
    <div class="container">
      <div class="item">
        <div class="pic">
          <img src="https://picsum.photos/400/400/?random=1" />
        </div>
        <div class="txt">
          <h2>金魚都能懂的網頁入門</h2>
          <p>每天都說很常見，啊就真的很常見呀~~XD</p>
          <a href="" class="btn">more</a>
        </div>
      </div>
      <div class="item">
        <div class="pic">
          <img src="https://picsum.photos/400/400/?random=2" />
        </div>
        <div class="txt">
          <h2>金魚都能懂的網頁入門</h2>
          <p>每天都說很常見，啊就真的很常見呀~~XD</p>
          <a href="" class="btn">more</a>
        </div>
      </div>
      <div class="item">
        <div class="pic">
          <img src="https://picsum.photos/400/400/?random=3" />
        </div>
        <div class="txt">
          <h2>金魚都能懂的網頁入門</h2>
          <p>每天都說很常見，啊就真的很常見呀~~XD</p>
          <a href="" class="btn">more</a>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped type="text/css">
.wrap {
  height: 100vh;
  display: flex;
  background: linear-gradient(-30deg, #fdaecb, #e7597f, #fe8556);
}

.container {
  width: 1200px;
  margin: auto;
  display: flex;
  flex-wrap: wrap;
}

.item {
  width: 368px;
  margin: 15px 15px;
  display: flex;
  background-color: #fff;
  border: 1px solid #888;
  box-shadow: 0 10px 30px rgba(160, 0, 0, 0.5);
}

.item .pic {
  width: 50%;
}

.item .pic img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.item .txt {
  width: 50%;
  padding: 20px;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
}

.item .txt h2 {
  margin-bottom: 0.4em;
  font-weight: 500;
}

.item .txt p {
  font-weight: 100;
}

.item .txt .btn {
  line-height: 1.5em;
  border: 1px solid #ccc;
  padding: 0 1em;
  align-self: flex-end;
  text-decoration: none;
  border-radius: 200px;
  margin-top: auto;
  color: #aaa;
}

.item .txt .btn:hover {
  background-color: #ccc;
  color: #fff;
}
</style>