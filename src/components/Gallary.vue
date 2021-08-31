<template>
  <div class="Gallary-wrapper clearfix">
    <div class="photolst-title"><p>叮！小虎表情包送到~</p></div>
    <div class="album">
    <div class="photo-wrap"><img src="../assets/p1.jpeg" alt="打哈欠"></div>
    <div class="photo-wrap" ><img src="../assets/p2.jpeg" alt="打哈欠"></div>
    <div class="photo-wrap" ><img src="../assets/p3.jpeg" alt="打哈欠"></div>
    <div class="photo-wrap"><img src="../assets/p10.jpeg" alt="打哈欠"></div>
    <div class="photo-wrap"><img src="../assets/p10.jpeg" alt="打哈欠"></div>
    <div class="photo-wrap"><img src="../assets/p10.jpeg" alt="打哈欠"></div>
    <div class="photo-wrap"><img src="../assets/p7.jpeg" alt="打哈欠"></div>
    <div class="photo-wrap"><img src="../assets/p8.jpeg" alt="打哈欠"></div>
    <div class="photo-wrap"><img src="../assets/p9.jpeg" alt="打哈欠"></div>
    </div>
    <br>
    <div class="copyrightrepo"><p>© 本相册版权归 <a href="">达闻西可颂</a> 所有，转载请联系作者。</p></div>
  </div>
</template>

<script>
export default {
  name: "Tora",
  components: {},
};
</script>

<style>
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
.Gallary-wrapper{
  width: 800px;
  height: 600px;
}
.photolst-title{
  width: 100%;
  margin: 0 auto;
  font-weight: bold;
  font-size: 16px;
  text-shadow:5px 5px 5px rgba(50, 145, 235,.5);
  margin: 5px;
}
.album{
  display:flex;
  flex-flow: row wrap;
  justify-content: space-around;
  padding: 0 10px;
}
.photo-wrap{
  width: 200px;
  height: 200px;
  overflow: hidden;
  border: 3px solid cornflowerblue;
}
.copyrightrepo{
  float: left;
}
img{
   max-width:100%; 
   object-fit: fill;
   /* object-fit使用 */
}

.clearfix{
  content:"";
  display: table;
  clear: both;
}

</style>