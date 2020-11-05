<template>
  <div class="side-menu">
    <form action="">
      <input type="search" placeholder="請輸入關鍵字" />
      <button>
        <fa class="fa" :icon="faSearch"></fa>
      </button>
    </form>
    <nav>
      <a href="#">
        <fa class="fa" :icon="faUsers"></fa>
        鐵人賽</a
      >
      <a href="#">
        <fa class="fa" :icon="faGavel"></fa>
        暴力班</a
      >
      <a href="#">
        <fa class="fa" :icon="faObjectGroup"></fa>
        RWD醬子</a
      >
      <a href="#">
        <fa class="fa" :icon="faGlobe"></fa>
        金魚網頁</a
      >
      <a href="#">
        <fa class="fa" :icon="faUtensils"></fa>
        金魚切版</a
      >
    </nav>
  </div>
</template>

<script>
import { faUsers } from "@fortawesome/free-solid-svg-icons";
import { faGavel } from "@fortawesome/free-solid-svg-icons";
import { faObjectGroup } from "@fortawesome/free-solid-svg-icons";
import { faGlobe } from "@fortawesome/free-solid-svg-icons";
import { faUtensils } from "@fortawesome/free-solid-svg-icons";
import { faSearch } from "@fortawesome/free-solid-svg-icons";
export default {
  computed: {
    faUsers() {
      return faUsers;
    },
    faGavel() {
      return faGavel;
    },
    faObjectGroup() {
      return faObjectGroup;
    },
    faGlobe() {
      return faGlobe;
    },
    faUtensils() {
      return faUtensils;
    },
    faSearch() {
      return faSearch;
    },
  },
};
</script>

<style type="test/css">
html,
body {
  height: 100%;
}
body {
  background-color: #546377;
}
.side-menu {
  width: 300px;
  height: 100%;
  background-image: linear-gradient(0deg, #3381b0, #c2196c);
  display: flex;
  flex-direction: column;
  padding: 50px 0;
  box-sizing: border-box;
  box-shadow: 5px 0px 10px hsla(240, 40%, 15%, 0.6);
}
.side-menu form {
  display: flex;
  padding: 5px 10px;
  margin-bottom: 50px;
  border-radius: 200px;
  border: 1px solid rgba(255, 255, 255, 0.4);
}
.side-menu form button,
.side-menu form input {
  border: none;
  padding: 5px 10px;
  color: #fff;
  outline: none;
  background-color: transparent;
}
.side-menu form input {
  width: 230px;
}
.side-menu form input::placeholder {
  color: #aaa;
}
.side-menu form button {
  width: 50px;
}
.side-menu nav a {
  display: block;
  padding: 10px;
  color: #fff;
  text-decoration: none;
  position: relative;
}
.side-menu nav a + a::before {
  content: "";
  position: absolute;
  border-top: 1px solid rgba(255, 255, 255, 0.4);
  left: 10px;
  right: 10px;
  top: 0;
}
.side-menu nav a .fa {
  margin-right: -1.1em;
  transform: scale(0);
  transition: 0.3s;
}
.side-menu nav a:hover .fa {
  margin-right: 0em;
  transform: scale(1);
}
</style>