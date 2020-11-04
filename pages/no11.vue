<template>
  <div class="wrap">
    <div class="item">
      <div class="icon">
        <fa class="fa" :icon="faGavel" />
      </div>
      <div class="txt">
        <h3>暴力網頁入門</h3>
        <p>
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sapiente,
          assumenda at! Pariatur omnis beatae voluptas! Debitis quidem minima
          consequuntur? Aliquid?
        </p>
      </div>
    </div>
    <div class="item">
      <div class="icon">
        <fa class="fa" :icon="faThumbsUp" />
      </div>
      <div class="txt">
        <h3>金魚都懂的切版</h3>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolores
          quisquam deleniti quo, tenetur culpa quam et ipsa eveniet fugiat natus
          nostrum molestiae voluptas sit, corporis dicta impedit. Optio earum
          velit provident ipsum?
        </p>
      </div>
    </div>
    <div class="item">
      <div class="icon">
        <fa class="fa" :icon="faBell" />
      </div>
      <div class="txt">
        <h3>超好吃稀飯飯</h3>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt est
          illo excepturi porro. Explicabo corporis qui, odio porro excepturi
          facilis fugiat sint perspiciatis pariatur architecto esse dolore
          deleniti sequi fuga ratione quaerat nostrum consequuntur nam libero ea
          atque quam reiciendis.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import { faGavel } from "@fortawesome/free-solid-svg-icons";
import { faThumbsUp } from "@fortawesome/free-solid-svg-icons";
import { faBell } from "@fortawesome/free-solid-svg-icons";
export default {
  computed: {
    faGavel() {
      return faGavel;
    },
    faThumbsUp() {
      return faThumbsUp;
    },
    faBell() {
      return faBell;
    },
  },
};
</script>

<style type="text/css">
html,
body {
  height: 100%;
  display: flex;
  align-items: center;
  background-image: linear-gradient(-45deg, #fffaf0, #f8c3c1);
}

.wrap {
  padding-top: 75px;
  width: 1200px;
  display: flex;
  margin: 100px auto;
}

.item {
  width: 370px;
  margin: 0 15px;
  text-align: center;
  border: 10px solid #f9cec2;
  background-color: #fff;
  border-radius: 20px;
  box-shadow: 10px 20px 50px #f7b6a7;
}

.item h3 {
  color: #f5afac;
}

.item p {
  color: #ccc;
}

.item .txt {
  padding: 20px 20px 2em;
}

.item .icon {
  width: 150px;
  height: 150px;
  background-color: #fff;
  margin: -75px auto 0;
  font-size: 85px;
  line-height: 150px;
  border-radius: 50%;
  color: #f5afac;
  position: relative;
}

.item .icon:before {
  content: "";
  width: 100%;
  height: 100%;
  position: absolute;
  border-top: 10px solid #f9cec2;
  border-right: 10px solid #f9cec2;
  border-bottom: 10px solid transparent;
  border-left: 10px solid transparent;
  top: -10px;
  left: -10px;
  border-radius: 50%;
  transform: rotate(-45deg);
}

.item:hover .fa {
  animation: ss 0.3s linear infinite alternate;
}

@keyframes ss {
  0% {
    transform: rotate(-10deg);
  }
  100% {
    transform: rotate(10deg);
  }
}
</style>