<template>
  <div class="main-header">
    <div class="container">
      <a href="" class="logo">
        <img src="" alt="" />
      </a>
      <div class="main-nav">
        <a href="#">金魚都能懂的系列</a>
        <a href="#">暴力網頁入門系列</a>
        <a href="#">CSS王可樂系列</a>
        <a href="#">RWD原來是醬子系列</a>
      </div>
      <div class="header-search">
        <input type="search" />
        <button type="submit">
          <fa :icon="faSearch" />
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import { faSearch } from "@fortawesome/free-solid-svg-icons";
export default {
  computed: {
    faSearch() {
      return faSearch;
    },
  },
};
</script>
<style scoped type="text/css">
.main-header {
  background: linear-gradient(0deg, #fe70d8, #3713c1);
}

.main-header .container {
  display: flex;
  padding: 20px;
  max-width: 1200px;
  justify-content: center;
  align-items: center;
}

.main-header .log {
  width: 100px;
}

.main-header .log img {
  width: 100%;
  vertical-align: middle;
}

.main-header .main-nav {
  margin: auto;
  display: flex;
}

.main-header .main-nav a:hover {
  transform: translateY(-5px);
}

.main-header .main-nav a {
  color: #fff;
  text-decoration: none;
  padding: 5px 1em;
  position: relative;
  transform: translateY(0px);
  transition: 0.3s;
}

.main-header .main-nav a:after {
  content: "";
  position: absolute;
  height: 0;
  left: 50%;
  right: 50%;
  border-bottom: 1px solid #fff;
  bottom: -5px;
  transition: 0.3s;
}

.main-header .main-nav a:hover:after {
  left: 0;
  right: 0;
}

.main-header .header-search {
  display: flex;
}

.main-header .header-search input,
.main-header .header-search button {
  border: none;
  background-color: #fff;
  padding: 5px 10px;
}

.main-header .header-search input:focus,
.main-header .header-search button:focus {
  outline: none;
}

.main-header .header-search input {
  border-radius: 200px 0 0 200px;
}

.main-header .header-search button {
  border-radius: 0 200px 200px 0;
}
</style>