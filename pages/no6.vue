<template>
  <div class="main-footer">
    <div class="container">
      <div class="footer-item">
        <nav>
          <h4>關於我們</h4>
          <a href="#"><fa :icon="faAngleRight" /> 課程目標</a>
          <a href="#"><fa :icon="faAngleRight" /> 辨學理念</a>
          <a href="#"><fa :icon="faAngleRight" /> 課程宗旨</a>
        </nav>
      </div>
      <div class="footer-item">
        <nav>
          <h4>課程列表</h4>
          <a href="#"><fa :icon="faAngleRight" /> 網頁建置入門</a>
          <a href="#"><fa :icon="faAngleRight" /> RWD網頁建置入門</a>
          <a href="#"><fa :icon="faAngleRight" /> CSS3互動動畫設計</a>
          <a href="#"><fa :icon="faAngleRight" /> Bootstrap框架實務</a>
        </nav>
      </div>
      <div class="footer-item">
        <nav>
          <h4>服務項目</h4>
          <a href="#"><fa :icon="faAngleRight" />網站建置顧問</a>
          <a href="#"><fa :icon="faAngleRight" />網站設計建置</a>
          <a href="#"><fa :icon="faAngleRight" />網站規劃</a>
          <a href="#"><fa :icon="faAngleRight" />企業教育訓練</a>
        </nav>
      </div>
      <div class="footer-item footer-subs">
        <h4>訂閱我們</h4>
        <form action="">
          <input type="text" name="" />
          <input type="submit" value="訂閱" />
        </form>
      </div>
    </div>
    <div class="copyright">Copy &copy; 2020 金魚稀飯版</div>
  </div>
</template>

<script>
import { faAngleRight } from "@fortawesome/free-solid-svg-icons";
export default {
  computed: {
    faAngleRight() {
      return faAngleRight;
    },
  },
};
</script>

<style scoped type="text/css">
.main-footer .container {
  display: flex;
  width: 1200px;
  margin: auto;
}
.main-footer {
  margin-top: 150px 0 0;
  background: linear-gradient(-20deg, #3f5494, #08c7a5);
}

.footer-item {
  width: 0;
  flex-grow: 1;
  margin: 20px;
}

.footer-item nav {
  display: flex;
  flex-direction: column;
}

.footer-item h4 {
  font-size: 24px;
  color: #fff;
  border-bottom: 1px dotted #fff;
  margin-bottom: 0.5em;
  margin-top: 0.5em;
}

.footer-item nav a {
  color: #fff;
  line-height: 1.4;
  text-decoration: none;
  padding: 5px 0;
}

.footer-item nav a:hover {
  color: #fa0;
}

.footer-subs {
  display: flex;
  flex-direction: column;
}

.footer-subs form {
  display: flex;
  width: 100%;
  margin: auto 0;
}

.footer-subs input[type="text"],
.footer-subs input[type="submit"] {
  border: none;
  display: 5px 10px;
}

.footer-subs input[type="text"] {
  width: 0;
  flex-grow: 1;
}

.footer-subs input[type="submit"] {
  color: #70f6df;
  background-color: #3e5293;
}

.copyright {
  width: 100%;
  text-align: center;
  margin: 150px 0;
  padding: 10px 0px;
  background-color: #3e5293;
  color: #70f6df;
}
</style>