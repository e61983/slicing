<template>
  <div class="table">
    <table>
      <caption>
        範列一覽表
      </caption>
      <thead>
        <tr>
          <th scope="col">基本版圖</th>
          <th scope="col">稀飯版版圖</th>
          <th scope="col">圖版</th>
          <th scope="col">選單</th>
          <th scope="col">表單</th>
          <th scope="col">表格</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><a href="no1">圖文滿版</a></td>
          <td><a href="no3">互動漂浮版</a></td>
          <td>敬請期待</td>
          <td><a href="no8">導覽列</a></td>
          <td>敬請期待</td>
          <td>敬請期待</td>
        </tr>
        <tr>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
        </tr>
        <tr>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
        </tr>
        <tr>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
        </tr>
        <tr>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
        </tr>
        <tr>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
          <td>敬請期待</td>
        </tr>
      </tbody>
      <tfoot>
        <tr>
          <td>備註</td>
          <td colspan="5">以上資料經什麼什麼的同意轉貼</td>
        </tr>
      </tfoot>
    </table>
  </div>
</template>

<style type="text/css">
html,
body {
  height: 100%;
}
body {
  display: flex;
  align-items: center;
  justify-content: center;
  background-image: linear-gradient(90deg, #3d5894, #08c7a5);
}
.table {
  width: 800px;
  margin: auto;
}
.table table {
  width: 100%;
  border: 3px double #666;
  background-color: #fff;
  border-radius: 10px;
}
.table thead {
  background-color: #333;
  color: #fff;
}
.table table th:first-child {
  border-radius: 7px 0 0 0;
}
.table table th:last-child {
  border-radius: 0 7px 0 0;
}
.table tbody a {
  color: #666;
}
.table tbody tr:nth-child(even) {
  background-color: #ffa;
}
.table table tfoot td:first-child {
  border-radius: 0 0 0 7px;
}
.table table tfoot td:last-child {
  border-radius: 0 0 7px 0;
}
.table tbody tr:hover {
  background-color: #fee;
}
.table tbody tr td:hover {
  background-color: #efe;
}
.table tbody td a{
    text-decoration: none;
}
.table tbody td:hover a{
    text-decoration: underline;
}
.table th {
  border: 1px solid #666;
  padding: 6px 10px;
}
.table td {
  border: 1px solid #666;
  padding: 6px 10px;
}
.table caption {
  caption-side: bottom;
  text-align: right;
  padding: 0 10px;
  color: #ccc;
}
</style>