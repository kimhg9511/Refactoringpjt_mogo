<template>
  <div class="story-about-us">
    <art-title></art-title>
    <span class="contents grey">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</span>
    <div class="image-cards">
      <div class="image-card bg-cyan">
        <img src="../images/story_about_us/story_about_us_1.png" alt="">
      </div>
      <div class="image-card bg-cyan">
        <img src="../images/story_about_us/story_about_us_2.png" alt="">
      </div>
      <div class="image-card bg-cyan">
        <img src="../images/story_about_us/story_about_us_3.png" alt="">        
      </div>
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
  display: flex;
  flex-direction: column;
  align-items: center;
}
.contents{
  width: 50%;
  font-family: Roboto;
  font-size: 1.5rem;
  line-height: 1.6;

  margin: 47px 0 100px;
}
.image-cards {
  min-width: 1280px;
  display: flex;
  justify-content: center;
}
.image-card {
  width: 380px;
  height: 250px;
  margin: 0 15px;
  position: relative;
}
.image-card>img{
  position: absolute;
  top: 0;
  left: 0;
  /* top: -10px; */
  /* left: -10px; */
}
</style>