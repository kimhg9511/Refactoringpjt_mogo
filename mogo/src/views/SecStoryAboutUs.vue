<template>
  <div class="section story-about-us">
    <div class="subtitle">What we do</div>
    <div class="title">STORY ABOUT US</div>
    <hr class="underline bg-red">
    <!-- 
    <span class="contents">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</span><br>
    <div class="image-card">
      <div class="selected">
        <img src="" alt="">
        <span class="super-team">SUPER&nbsp;TEAM</span>
      </div>
    </div>
    <div class="image-card">
      <img src="" alt="">
    </div>
    <div class="image-card">
      <img src="" alt="">
    </div> -->
  </div>
</template>

<script>
export default {

}
</script>

<style>
.story-about-us{
  text-align: center;
  height: 750px;
  position: relative;
}
.subtitle {
  height: 23px;
  font-family: KaushanScript;
  font-size: 2.4rem;
  line-height: 2.4rem;
  text-align: center;

  position: absolute;
  top:12%;
  left: 50%;
  transform: translateX(-50%);
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
  left: 50%;
  transform: translateX(-50%);
}
.underline{
  position: absolute;
  top: 26.6667%;
  left: 50%;
  transform: translateX(-50%);
}
.story-about-us>.contents{
    width: 954px;
    height: 39px;
    font-family: Roboto;
    font-size: 15px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.6;
    letter-spacing: normal;
    text-align: center;
    color: #999999;
    line-height: 19.5px;
    margin: 0 auto 101px;
}
.USERS {
    width: 32px;
    height: 24px;
    background-color: #ffffff;
}
.selected>img{
  display: block;
  margin: 103px auto 11px;
}
.super-team {
    font-family: Montserrat;
    font-size: 18px;
    font-weight: bold;
    font-stretch: normal;
    font-style: normal;
    line-height: normal;
    letter-spacing: normal;
    text-align: center;
    color: #ffffff;
    /**/
    line-height: 14px;
}
.image-card {
    width: 380px;
    height: 250px;
    background-color: #95e1d3;/* need to change */
    display: inline-block;
    margin: 0 15px 110px;
    position: relative;
}
.image-card>img{
  float: left;
}
</style>