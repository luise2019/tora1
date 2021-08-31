<template>
    <div class="top-bar-wrapper clearfix">
      <div class="top-bar clearfix">
        <div class="location">
          <div class="city">
            <i class="fa fa-map-marker"></i>&nbsp;
            <a href="#">北京</a>
          </div>
          <div class="city-list"></div>
        </div>
        <ul class="short-cut">
          <li>
            <a href="http://" target="_blank">你好，请登录</a>
            &nbsp;&nbsp;
            <a class="style-red" href="http://" target="_blank">免费注册</a>
          </li>
          <li class="spacer"></li>
          <li><a href="http://" target="_blank">我的订单</a></li>
          <li class="spacer"></li>
          <li>
            <a href="http://" target="_blank">我的京东</a>
            &nbsp;<i class="fa fa-angle-down"></i>
          </li>
          <li class="spacer"></li>
          <li><a href="http://" target="_blank">京东会员</a></li>
          <li class="spacer"></li>
          <li>
            <a class="style-red" href="http://" target="_blank">企业采购</a>
            &nbsp;<i class="fa fa-angle-down"></i>
            <span></span>
          </li>
          <li class="spacer"></li>
          <li>客户服务 &nbsp;<i class="fa fa-angle-down"></i></li>
          <li class="spacer"></li>
          <li>网站导航 &nbsp;<i class="fa fa-angle-down"></i></li>
          <li class="spacer"></li>
          <li>手机京东</li>
        </ul>
      </div>
    </div>
</template>

<script>
export default {
  name: "TopBar",
  props: {
  },
};
</script>

<style>
* {
  margin: 0 auto;
  padding: 0;
}
body {
  font: 12px/1.5 Microsoft YaHei, Heiti SC, tahoma, arial, Hiragino Sans GB,
    "\5B8B\4F53", sans-serif;
}
.top-bar-wrapper {
  width: 100%;
  background-color: #e3e4e5;
  /*  */
  line-height: 29px;
  height: 30px;
  border-bottom: 1px #ddd solid;
}
.top-bar {
  width: 1190px;
  margin: 0px auto;
  position: relative;
  top:0px;
  left: 0px;
}
.location {
  float: left;
  font-size: 12px;
}
.city{
  padding: 0 10px;
  /* 调整兄弟元素层级，用city盖住下方的菜单 */
  border:1px solid transparent;
  border-bottom: none;
  position: relative;
  z-index: 999;
}
/* 城市菜单，默认不显示 */
.location .city-list{
  display: none;
  width: 320px;
  height: 436px;
  background-color: #ffffff;
  border: 1px solid rgb(204,204,204);
  /* 固定定位，不影响其他元素 */
  position: absolute;
  top:30px;
  box-shadow: 0px 2px 2px rgba(0,0,0,.2);
}
/* 移入location时显示 */
.location:hover .city-list {
  display: block;
}

.location:hover .city{
  background-color: #ffffff;
  border: 1px solid rgb(204,204,204);
  border-bottom:none;
  padding-bottom: 1px;
} 
.city .fa {
  font-size: 14px;
  color: #ff0000;
  margin-right: 4px;
}
.short-cut {
  float: right;
  font-size: 12px;
}
.short-cut .style-red{
  color:#ff0000
}
.short-cut li {
  float: left;
}
.short-cut .spacer {
  width: 2px;
  height: 10px;
  /* 显示不出来？ */
  color: #2c3e50;
  margin: 10px 5px 0;
  overflow: hidden;
}


.clearfix::before,
.clearfix::after {
  content: " ";
  clear: both;
  display: table;
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
</style>