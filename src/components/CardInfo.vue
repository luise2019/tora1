<template>
  <div class="outer clearfix">
    <div class="card">
      <div class="img-wrapper">
        <img src="../assets/p10.jpeg" alt="Tora头像" srcset="" />
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
          <li class="fa fa-star"></li>
        </ul>
        <a class="share" href=""><span class="fa fa-weibo"></span></a>
      </div>
    </div>
    <div class="EmbedVideo">
        <video id="video-cat"
          src="../assets/p57180325.mp4"
          controls
          poster="../assets/p206202201.jpg"
        ></video>
      <div class="video-msg">
        <p class="video-des">其他猫喵喵喵</p>
        <p class="video-intro">放个视频嗷呜嗷呜🐖</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardInfo",
  components: {},
};
</script>

<style>
.outer {
  width: 600px;
}
.card,
.EmbedVideo {
  float: left;
  border-bottom-right-radius: 0.5em;
  border-bottom-left-radius: 0.5em;
  box-shadow: 2px 2px 0.5em grey, -2px -2px 0.5em grey;
  text-align: left;
}
.card {
  width: 150px;
}
.img-wrapper {
  width: 100%;
}
.img-text {
  color: #717171;
  padding: 0 10px;
}
.img-title {
  font-size: 18px;
}
.img-des::before {
  content: "❤";
}
.img-intro,
.img-des {
  margin-top: 3px;
  margin-bottom: 5px;
  font-size: 13px;
  line-height: 15px;
}
.star-wrapper {
  height: 30px;
  line-height: 30px;
  display: flex;
  border-top: 1px solid #717171;
  padding: 0 10px;
}
/* 弹性项目两边对齐 */
.star {
  align-self: flex-start;
  margin-left: 0;
}
.share {
  margin-right: 0;
}
.EmbedVideo {
  width: 400px;
  margin-left: 10px;
}
#video-cat {
  width: 100%;
}
.video-msg {
  font-size: 15px;
  border-top: 1px solid #717171;
  padding-left: 10px;
  padding-top: 10px;
  padding-bottom: 10px;
}
img {
  max-width: 100%;
}
</style>