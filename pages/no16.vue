<template>
  <div class="wrap">
    <ol class="list">
      <li>
        <div class="pic">
          <fa class="fa" :icon="faFileImport" />
          <div class="txt">
            <h3>收到訂單</h3>
          </div>
        </div>
      </li>
      <li class="active">
        <div class="pic">
          <fa class="fa" :icon="faFileArchive" />
          <div class="txt">
            <h3>揀貨中</h3>
          </div>
        </div>
      </li>
      <li>
        <div class="pic">
          <fa class="fa" :icon="faTruck" />
          <div class="txt">
            <h3>運送中</h3>
          </div>
        </div>
      </li>
      <li>
        <div class="pic">
          <fa class="fa" :icon="faCheckCircle" />
          <div class="txt">
            <h3>已送達</h3>
          </div>
        </div>
      </li>
    </ol>
  </div>
</template>
<script>
import {
  faFileImport,
  faFileArchive,
  faTruck,
  faCheckCircle,
} from "@fortawesome/free-solid-svg-icons";
export default {
  computed: {
    faFileImport() {
      return faFileImport;
    },
    faFileArchive() {
      return faFileArchive;
    },
    faTruck() {
      return faTruck;
    },
    faCheckCircle() {
      return faCheckCircle;
    },
  },
};
</script>

<style type="text/css">
html,
body {
  height: 100%;
}
body {
  background-color: #546377;
}
.wrap {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
}
.list {
  width: 100%;
  display: flex;
  justify-content: center;
}
.list li {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  width: 150px;
  height: 150px;
  background-image: linear-gradient(9deg, #185a9d, #43cea2);
  border-radius: 50%;
  position: relative;
  font-size: 25px;
  color: #fff;
  box-shadow: 0px 0px 0px 4px #fff;
}
.list li .fa {
  font-size: 50px;
  margin-bottom: 6px;
}
.list li + li {
  margin-left: 100px;
}
.list li + li::before {
  content: "";
  position: absolute;
  width: 100px;
  height: 5px;
  top: 0;
  bottom: 0;
  margin: auto;
  left: -100px;
  background-image: linear-gradient(9deg, #185a9d, #43cea2);
  z-index: -1;
  box-shadow: 0px 0px 0px 3px #fff;
}
.list li.active ~ li {
  background-image: linear-gradient(9deg, #999, #ccc);
}

.list li.active ~ li::before {
  background-image: linear-gradient(9deg, #999, #ccc);
}
</style>