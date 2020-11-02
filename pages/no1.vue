<template>
  <div class="banner">
    <div class="container">
      <div class="banner-txt">
        <h1>
          金魚都能懂的
          <small>這個畫面怎麼切</small>
        </h1>
        <h2>圖文滿版區塊</h2>
        <p>
          這個畫面實在常見，在個種樣版網站中可說是常客
          <br />
          金魚切不出來實在說不過去啊
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>


<style scoped type="text/css">
* {
  margin: 0;
  padding: 0;
  list-style: none;
}

.banner {
  width: 100%;
  height: 100vh;
  background: linear-gradient(115deg, #7bf, 50%, transparent 50%) center center /
      100% 100%,
    url("https://picsum.photos/1200/600?random=10") right center / auto 100%;
}

.container {
  width: 1200px;
  height: 100%;
  margin: auto;
}
.banner-txt {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
}
.banner-txt h1 {
  font-size: 80px;
  border-bottom: 1px solid #ccc;
  margin-bottom: 0.3em;
  padding-bottom: 0.3em;
}
.banner-txt h1 small {
  display: block;
  font-size: 53px;
}
.banner-txt h2 {
  font-size: 50px;
}
.banner-txt p {
  font-size: 20px;
}
</style>