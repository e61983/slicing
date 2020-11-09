<template>
  <div
    class="container d-flex min-vw-100 flex-column flex-md-row justify-content-center"
  >
    <div class="wrap m-3 p-2" v-for="(item, index) in items" :key="index">
      <div
        class="header justify-content-center"
        :style="{ backgroundImage: `url(${backgroundUrl})` }"
      >
        <div class="d-flex justify-content-center align-items-center">
          <div class="w-100 flex-column align-items-center">
            <div class="">
              <div class="pic">
                <img
                  :src="'https://picsum.photos/1400/900/?random=5' + index"
                />
              </div>
            </div>
            <div class="d-flex justify-content-end">
              <div class="txt">
                <h3>{{ item.title }}</h3>
                <p>{{ item.subtitle }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row content">
        <div class="col-12">
          <h3><fa class="fa" :icon="faCircleNotch" />特色</h3>
          <ul>
            <li v-for="(feature, index) in item.features" :key="index">
              <fa class="fa" :icon="faCircle" />{{ feature }}
            </li>
          </ul>
        </div>
        <div class="col-12">
          <h3><fa class="fa" :icon="faCircleNotch" />種類</h3>
          <ul class="d-flex flex-wrap">
            <li v-for="(c, index) in item.classes" :key="index">
              <fa class="fa" :icon="faCircle" />{{ c }}
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import bgHeader from "@/assets/bg-header.png";
import { faCircle, faCircleNotch } from "@fortawesome/free-solid-svg-icons";
export default {
  data() {
    return {
      items: [
        {
          title: "吃比瘦更有福",
          subtitle: "減肥永遠是明天的事",
          features: [
            "特別好吃又好玩",
            "一定要來試試的餅乾",
            "走過路過千萬別錯過",
            "是千年一遇的甜點",
          ],
          classes: ["麵包", "吐司", "餅乾", "蛋糕", "鬆餅", "千層餅"],
        },
        {
          title: "甜點才是王道",
          subtitle: "來點茶也是挺好的",
          features: [
            "特別好喝又好玩",
            "一定要來試試的紅茶",
            "走過路過千萬別錯過",
            "是千年一遇的春天",
          ],
          classes: ["經典紅茶", "夏日伯爵", "哈爾濱的春天", "尉藍之秋"],
        },
      ],
    };
  },
  computed: {
    backgroundUrl() {
      return bgHeader;
    },
    faCircleNotch() {
      return faCircleNotch;
    },
    faCircle() {
      return faCircle;
    },
  },
};
</script>

<style scoped type="text/css">
.wrap {
  width: 300px;
}
.header {
  margin: 0 -15px;
  background-color: #ccc;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: 0 20%;
  object-fit: cover;
}
.pic {
  width: 85%;
  margin: 20px auto 0;
  border-radius: 100%;
  overflow: hidden;
}
.pic img {
  width: 100%;
  vertical-align: middle;
}
.txt {
  width: 60%;
  margin: 20px 0 0 0;
  padding: 10px 0;
  position: relative;
  text-align: right;
  z-index: 3;
}
.txt h3 {
  font-size: 28px;
}
.txt p {
  font-size: 15px;
}
.txt::after {
  position: absolute;
  content: "";
  width: 0;
  height: 0;
  bottom: 0;
  top: -25px;
  right: 0;
  margin: auto;
  border-style: solid;
  border-width: 100px 200px 100px 0;
  border-color: transparent #eee transparent transparent;
  z-index: -1;
}

.txt::before {
  position: absolute;
  content: "";
  width: 0;
  height: 0;
  bottom: 0;
  top: -15px;
  right: 0;
  margin: auto;
  border-style: solid;
  border-width: 100px 200px 100px 0;
  border-color: transparent #5b3878 transparent transparent;
  z-index: -1;
}
.content {
  background-color: #eee;
  padding: 20px 10px;
}
.content h3 {
  margin-bottom: 10px;
}
.content ul li {
  padding: 0 20px;
}
.content h3 .fa {
  font-size: 25px;
  padding-right: 5px;
}
.content ul li .fa {
  font-size: 10px;
  padding-right: 5px;
}
</style>