<template>
  <div class="story-about-us">
    <art-title></art-title>
    <span class="contents">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</span>
    <div class="image-card-wrap">
      <img src="../images/story_about_us/story_about_us_1.png" alt="" class="image-card bg-cyan">
      <img src="../images/story_about_us/story_about_us_2.png" alt="" class="image-card bg-cyan">
      <img src="../images/story_about_us/story_about_us_3.png" alt="" class="image-card bg-cyan">
    </div>
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

<style scoped>
.story-about-us{
  text-align: center;
  height: 750px;
  position: relative;
}
/* align center */
.story-about-us>*{
  left: 50%;
  transform: translateX(-50%);  
}

.underline{
  position: absolute;
  top: 26.6667%;
  /* left: 50%;
  transform: translateX(-50%); */
}
.contents{
  width: 50%;
  height: 40px;
  font-family: Roboto;
  font-size: 1.5rem;
  line-height: 1.6;
  text-align: center;
  color: #999999;

  position: absolute;
  top: 33%;
  /* left: 50%;
  transform: translateX(-50%); */
}
.image-card-wrap {
  min-width: 1280px;
  position: absolute;
  bottom: 14.6668%;
}
.image-card {
  width: 380px;
  height: 250px;
  margin: 0 15px;
  display: inline-block;
}
.image-card>img{
  float: left;
}
</style>