<template>
  <div class="wrap">
    <div class="item">
      <img src="https://picsum.photos/500/500/?random=10" />
      <div class="txt">
        <div class="h3">金魚都懂切版</div>
        <div class="p">
          這是個問句，你會什麼? 這很重要，因為你可能是程式奇才而不適合切版呀~!
        </div>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/500/500/?random=11" />
      <div class="txt">
        <div class="h3">金魚都懂切版</div>
        <div class="p">
          這是個問句，你會什麼? 這很重要，因為你可能是程式奇才而不適合切版呀~!
        </div>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/500/500/?random=12" />
      <div class="txt">
        <div class="h3">金魚都懂切版</div>
        <div class="p">
          這是個問句，你會什麼? 這很重要，因為你可能是程式奇才而不適合切版呀~!
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Natus,
          alias.
        </div>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/500/500/?random=13" />
      <div class="txt">
        <div class="h3">金魚都懂切版</div>
        <div class="p">
          這是個問句，你會什麼? 這很重要，因為你可能是程式奇才而不適合切版呀~!
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fuga non
          aspernatur similique ipsam! A, tenetur dolor?
        </div>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/500/500/?random=14" />
      <div class="txt">
        <div class="h3">金魚都懂切版</div>
        <div class="p">
          這是個問句，你會什麼? 這很重要，因為你可能是程式奇才而不適合切版呀~!
        </div>
      </div>
    </div>
  </div>
</template>

<style text="text/css">
body {
  background-color: #000;
}
.wrap {
  width: 100%;
  margin: auto;
  overflow: hidden;
}
.item {
  float: left;
  position: relative;
}

.item img {
  width: 100%;
  vertical-align: middle;
  object-fit: cover;
}

.item:first-child {
  width: 50%;
}

.item:first-child ~ .item {
  width: 25%;
}

.item .txt {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 15px;
  color: #fff;
  background-color: rgba(0, 0, 0, 0.6);
  box-sizing: border-box;
  display: flex;
  opacity: 0;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: 0.5s;
  transform: scale(0);
}

.item h3 {
  margin-bottom: 0.4em;
}

.item p {
  font-weight: 100;
  line-height: 1.7em;
}
.item:hover .txt {
  opacity: 100%;
  transform: scale(1);
}
</style>