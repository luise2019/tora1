<template>
  <div class="outer">
    <div class="img-wrapper">
        <img src="../assets/p10.jpeg" alt="Tora头像" srcset="">
    </div>
    <div class="img-text">
        <p class="img-title">虎哥</p>
        <p class="img-des">&nbsp;公橘</p>
        <p class="img-intro">虎哥委屈巴巴嗷呜嗷呜，要麻麻起床看它🙈</p>
    </div>
    <div class="star-wrapper">
        <ul class="star">
            <li class="fa fa-star"></li>
            <li class="fa fa-star"></li>
            <li class="fa fa-star"></li>
            <li class="fa fa-star"></li>
        </ul>
        <a class="share" href=""><span class="fa fa-weibo"></span></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardInfo",
  components: { 
  },
};
</script>

<style>
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
.outer {
    width: 150px;
    margin-left: 55px;
    border-bottom-right-radius:.5em;
    border-bottom-left-radius:.5em;
    box-shadow: 2px 2px .5em grey,-2px -2px .5em grey;
}
.img-wrapper{
    width: 150px;
}
.img-text{
    text-align: left;
    color: #717171;
    padding: 0 10px;
}
.img-title{
    font-size: 18px;
}
.img-des::before{
    content:"❤";

}
.img-intro,.img-des{
    margin-top: 3px;
    margin-bottom: 5px;
    font-size: 13px;
    line-height: 15px;
}
.star-wrapper{
    height: 30px;
    line-height: 30px;
    display: flex;   
    border-top:1px solid #717171;
    padding: 0 10px;
}
/* 弹性项目两边对齐 */
.star{
    align-self:flex-start;
    margin-left: 0;
}
.share{
    margin-right: 0;
}
img{
   max-width:100%; 
}
</style>