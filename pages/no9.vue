<template>
  <div class="wrap">
    <ol class="breakcrumb">
      <li><a href="#">CSS可樂</a></li>
      <li><a href="#">CSS教學</a></li>
      <li><a href="#">金魚</a></li>
      <li><a href="#">切版技巧</a></li>
      <li><a href="#">Flex</a></li>
      <li><a href="#">麵包屑</a></li>
    </ol>
  </div>
</template>

<style type="text/css">
body {
  background-color: #562878;
}
.wrap {
  padding: 10px 0;
  background-color: #ec008b;
  box-shadow: 0px 5px 5px hsla(260, 100%, 20%, 0.5);
}
.breakcrumb {
  widows: 90%;
  margin: auto;
  display: flex;
}
.breakcrumb li {
  margin: 0 20px;
}
.breakcrumb a {
  text-decoration: none;
  color: #fff;
}
.breakcrumb li + li {
  padding-left: 0;
}
.breakcrumb li + li::before {
  content: ">";
  color: #fff;
  margin-right: 20px;
}
.breakcrumb li:last-child a,
.breakcrumb a:hover {
  color: #ff0;
}
</style>