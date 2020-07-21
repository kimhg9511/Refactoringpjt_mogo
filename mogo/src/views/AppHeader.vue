<template>
  <header 
    :style="{
      backgroundImage: `linear-gradient(to top, rgba(252,227,138,0.9), rgba(243,129,129,0.9)), url(${require('@/images/header_background.png')})`
    }"
    class="white"
  >
    <div class="logo">MoGo</div>
    <div class="nav-bar">
      <li class="nav-item">ABOUT</li>
      <li class="nav-item">SERVICE</li>
      <li class="nav-item">WORK</li>
      <li class="nav-item">BLOG</li>
      <li class="nav-item">CONTACT</li>
      <!-- <li class="nav-item"></li>
      <li class="nav-item"></li> -->
    </div>
    <div class="subtitle__header">
      Creative&nbsp;Template
    </div>
    <div class="title__header">
      WELCOME<br>TO&nbsp;MOGO
    </div>    
    <hr class="underline bg-white">
    <div class="learn-more">LEARN&nbsp;MORE</div>
    <div class="slide">
      <ul class="slide-name">
        <li class="slide-item"><span class="number">01</span>INTRO</li>
        <li class="slide-item"><span class="number">02</span>WORK</li>
        <li class="slide-item"><span class="number">03</span>ABOUT</li>
        <li class="slide-item"><span class="number">04</span>CONTACTS</li>
      </ul>
    </div>
  </header> 
</template>

<script>
export default {
}
</script>

<style scoped>
header {
  height: 1000px;
  background-size: 100% 100%;
  background-repeat: no-repeat;
  background-position: center;
  background-blend-mode: normal;
  position: relative;
}
.logo {
  font-family: Montserrat;
  font-size: 3rem;
  line-height: 3rem;
  font-weight: bold;
  text-align: left;

  position: absolute;
  top: 2.5%;
  left: 18.750%;
}
.nav-bar{
  position: absolute;
  top: 3.5%;
  right: 18.750%;
}
.nav-item{
  font-family: Montserrat;
  font-size: 1.4rem;
  font-weight: normal;
  text-align: center;

  display: inline-block;
  margin: 0 27.5px;
}
.subtitle__header {
  font-family: KaushanScript;
  font-size: 7.2rem;
  text-align: center;

  position: absolute;
  top: 23%;
  left: 50%;
  transform: translateX(-50%);
}
.title__header {
  font-family: Montserrat;
  font-size: 15rem;
  font-weight: bold;
  line-height: 15rem;
  letter-spacing: normal;
  text-align: center;

  position: absolute;
  top: 36%;
  left: 50%;
  transform: translateX(-50%);
}
header> .underline {
  position: absolute;
  bottom: 31%;
  left: 50%;
  transform: translateX(-50%);
}
.learn-more {
  width: 160px;
  height: 40px;
  font-family: Montserrat;
  font-size: 1.4rem;
  font-weight: bold;
  line-height: 4rem;
  text-align: center;
  border: 3px solid #ffffff;

  position: absolute;
  bottom: 23%;
  left: 50%;
  transform: translateX(-50%);
}
.slide{
  min-width: 1240px;
  text-align: center;
  position: absolute;
  bottom: 2.7%;
  left: 50%;
  transform: translateX(-50%);
}
.slide-item {
  width: 280px;
  font-family: Montserrat;
  font-size: 1.8rem;
  font-weight: 400;
  text-align: left;
  color: rgba(255,255,255, 0.7);

  line-height: 1.8rem;
  display: inline-block;
  margin: 0 15px;
  border-top: 3px solid rgba(255,255,255, 0.5);
  padding-top: 25px;
}
.slide-item>.number {
  font-size: 2.4rem;
  font-weight: bold;
  padding-right: 5px;
}
</style>