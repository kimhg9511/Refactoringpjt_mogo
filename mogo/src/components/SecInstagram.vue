<template>
  <div class="instagram">
    <p class="instagram-title">INSTAGRAM</p>
    <div class="photos">
      <img src="../images/sns/instagram_1.png" alt="">
      <img src="../images/sns/instagram_2.png" alt="">
      <img src="../images/sns/instagram_3.png" alt="">
      <img src="../images/sns/instagram_4.png" alt="">
      <img src="../images/sns/instagram_5.png" alt="">
      <img src="../images/sns/instagram_6.png" alt="">
      <img src="../images/sns/instagram_7.png" alt="">
      <img src="../images/sns/instagram_8.png" alt="">
      <img src="../images/sns/instagram_9.png" alt="">
    </div>
    <span class="view-more grey">view more photos</span>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.instagram{
  flex-shrink: 0;
  width: 270px;
}
.instagram-title {
  font-family: Montserrat;
  font-size: 1.4rem;
  font-weight: 500;
  margin-bottom: 40px;
}
.photos {
  display: flex;
  flex-wrap: wrap;
  margin-bottom: 20px;
}
.photos>img {
  width: 90px;
  border: 1px solid #fff;
}
.photos>img:nth-of-type(-n+3){
  border-top: 0;
}
.photos>img:nth-of-type(3n+1){
  border-left: 0;
}
.view-more {
  font-size: 1.3rem;
  font-weight: 300;
  font-style: italic;
  line-height: 1.85;
  text-align: left;
  line-height: 13px;
}
</style>