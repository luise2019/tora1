<template>
  <div id="app">
    <div class="top-bar-wrapper clearfix">
      <div class="top-bar clearfix">
        <div class="location">
          <div class="city">
            <a href="#">北京</a>
          </div>
        </div>

        <ul class="short-cut">
          <li>
            <a href="http://" target="_blank">你好，请登录</a>
            &nbsp;&nbsp;
            <a href="http://" target="_blank">免费注册</a>
          </li>
          <li class="spacer"></li>
          <li><a href="http://" target="_blank">我的订单</a></li>
          <li class="spacer"></li>
          <li><a href="http://" target="_blank">我的京东圈</a></li>
          <li class="spacer"></li>
          <li><a href="http://" target="_blank">京东会员</a></li>
            <li class="spacer"></li>
          <li>
            <a href="http://" target="_blank">企业采购</a>
            <span></span>
          </li>
          <li class="spacer"></li>
          <li>客户服务
            <span></span>
          </li>
          <li class="spacer"></li>
          <li>网站导航<span></span></li>
            <li class="spacer"></li>
          <li>手机京东</li>
        </ul>
      </div>
    </div>
    <h1>不要做菜狗</h1>

    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style>
* {
  margin: 0 auto;
  padding: 0;
}
body {
  color: #999;
  font: 12px/1.5 Microsoft YaHei, Heiti SC, tahoma, arial, Hiragino Sans GB,
    "\5B8B\4F53", sans-serif;
}
.top-bar-wrapper {
  width: 100%;
  background-color: #e3e4e5;
  line-height: 29px;
  height: 30px;
  border-bottom: 1px #ddd solid;
}
.top-bar {
  width: 850px;
  margin: 0px auto;
}
.location {
  float: left;
  font-size: 12px;
}
.short-cut {
  float: right;
  font-size: 12px;
}
.short-cut li {
  float: left;
}

.clearfix::before,
.clearfix::after {
  content: " ";
  clear: both;
  display: table;
}

.short-cut .spacer{
  width: 1px;
  height: 10px;
  background-color: #e3e4e5;
  margin: 10px 12px;
}
a {
  text-decoration: none;
  color: #2c3e50;
}
a:hover {
  color: #ff0000;
}
li {
  list-style: none;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
