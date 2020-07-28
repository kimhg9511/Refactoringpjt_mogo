<template>
  <div class="comment bg-f8">
    <img class="comment-left" src="../images/comment/left.png" alt="">
    <div class="comment-image">
      <img src="../images/comment/icon.png" alt="">
    </div>
    <div class="comment-contents">
      <div class="comment-text grey">"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. eiusmod tempor incididunt ut labore et dolore magna aliqua."</div>              
      <hr class="content-underline"><span class="comment-name">Jon Doe</span>
    </div>
    <img class="comment-right" src="../images/comment/right.png" alt="">
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.comment{
  height: 290px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 18.8%;
}
.comment-image {
  width: 150px;
  height: 150px;
  flex-shrink: 0;
  margin-left: 6.25%;
  border: solid 3px #95e1d3;

  /* 내부 이미지 중앙정렬 */
  display: flex;
  align-items: center;
  justify-content: center;
}
.comment-contents{
  width: 767px;
  height: 150px;
  flex-grow: 1;
  margin-left: 5%;
  margin-right: 6.25%;
}
.comment-text{
  margin-top: -5px;
  height: 106px;
  overflow: scroll;
  margin-bottom: 23px;
  font-family: Roboto;
  font-size: 2.4rem;
  font-weight: 300;
  font-style: italic;
  line-height: 1.5;
}
.content-underline{
  width: 60px;
  height: 3px;
  border: none;
  background-color: #f38181;
  display: inline-block;
}
.comment-name {
  font-family: KaushanScript;
  font-size: 2.4rem;
  line-height: 22px;
  margin-left: 10px;
}
.comment-left{
  margin-left: 1.9%;
}
.comment-right{
  margin-right: 1.9%;
}
</style>