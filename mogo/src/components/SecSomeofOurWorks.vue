<template>
  <div class="some_of_our_works">
    <art-title></art-title>
    <div class="comments">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    </div>
    <div class="image-wrap">
      <div class="images">
        <img src="../images/some_of_our_works/1.png" alt="">
        <img src="../images/some_of_our_works/2.png" alt="">
        <img src="../images/some_of_our_works/3.png" alt="">
        <img src="../images/some_of_our_works/4.png" alt="">
        <img src="../images/some_of_our_works/5.png" alt="">
        <img src="../images/some_of_our_works/6.png" alt="">
        <img src="../images/some_of_our_works/7.png" alt="">
      </div>
    </div>
    <!-- <div class="section comment-wrap">
      <div class="comment-content-wrap">
        <img class="carousel-left" src="../../static/mogo/img/mogo/mogo_carousel-left.png" alt="">
        <img class="carousel-right" src="../../static/mogo/img/mogo/mogo_carousel-right.png" alt="">
        <div class="comment-image">
          <img src="img/mogo/mogo_comment.png" alt="" class="small">
        </div>
        <div class="comment-comments">
          <span class="comment-text">"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. eiusmod tempor incididunt ut labore et dolore magna aliqua."</span>              
          <hr class="underline"><span class="comment-name">Joshua&nbsp;Earle</span>
        </div>
      </div>
    </div> -->
  </div>
</template>

<script>
import ArtTitle from './ArtTitle'
export default {
  components: {
    ArtTitle,
  }
}
</script>

<style>
.some_of_our_works {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}
.some_of_our_works>.comments {
  width: 954px;
  height: 39px;
  font-family: Roboto;
  font-size: 1.5rem;
  line-height: 1.6;
  margin: 46px 0 102px;
}
.images {
  padding: 0 auto;
  width: 100%;
  display: grid;
  grid-template-columns: repeat(2, 480px);
  grid-template-rows: repeat(4,390px);
  margin-bottom: 30px;
}
.images>img:nth-of-type(3){
  grid-row: span 2;
}
@media screen and (min-width: 1440px){
.images {
  grid-template-columns: repeat(3, 480px);
  grid-template-rows: repeat(3,390px); 
}
}
@media screen and (min-width: 1920px){
.images {
  grid-template-columns: repeat(4, 480px);
  grid-template-rows: repeat(2,390px); 
}
}
/* comment */
/* .some_of_our_works>.comment-wrap{
  padding-top: 15px;
  margin: 0;
  background-color: #ffffff;
}
.some_of_our_works>.comment-wrap>.comment-content-wrap>.comment-image{
  width: 210px;
  height: 210px;
  border: none;
}
.some_of_our_works .comment-text{
  margin-top: 40px;
} */
</style>