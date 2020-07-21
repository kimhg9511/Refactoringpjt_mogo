<template>
  <div class="story-about-us">
    <div class="subtitle">What we do</div>
    <div class="title">STORY ABOUT US</div>
    <hr class="underline bg-red">
    <span class="contents">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</span>
    <div class="card-wrap">
      <img src="" alt="" class="image-card bg-cyan">
      <img src="" alt="" class="image-card bg-cyan">
      <img src="" alt="" class="image-card bg-cyan">
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.story-about-us{
  text-align: center;
  height: 750px;
  position: relative;
}
.story-about-us>*{
  left: 50%;
  transform: translateX(-50%);  
}
.subtitle {
  height: 23px;
  font-family: KaushanScript;
  font-size: 2.4rem;
  line-height: 2.4rem;
  text-align: center;

  position: absolute;
  top:12%;
  /* left: 50%;
  transform: translateX(-50%); */
}
.title {
  height: 23px;
  font-family: Montserrat;
  font-size: 3rem;
  line-height: 3rem;
  font-weight: bold;
  text-align: center;

  position: absolute;
  top: 18.2668%;
  /* left: 50%;
  transform: translateX(-50%); */
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
.card-wrap {
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