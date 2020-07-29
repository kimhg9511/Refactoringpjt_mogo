<template>
  <header 
    :style="{
      backgroundImage: `linear-gradient(to top, rgba(252,227,138,0.9), rgba(243,129,129,0.9)), url(${require('@/images/header/bg.png')})`
    }"
    class="white"
  >
    <navigation-bar></navigation-bar>
    <div class="subtitle__header">
      Creative Template
    </div>
    <div class="title__header">
      WELCOME TO MOGO
    </div>    
    <hr class="underline bg-white">
    <div class="learn-more">LEARN MORE</div>
    <ul class="slides">
      <li class="slide"><span class="number">01</span>INTRO</li>
      <li class="slide"><span class="number">02</span>WORK</li>
      <li class="slide"><span class="number">03</span>ABOUT</li>
      <li class="slide"><span class="number">04</span>CONTACTS</li>
    </ul>
  </header> 
</template>

<script>
import NavigationBar from '../components/NavigationBar';

export default {
  components: {
    NavigationBar,
  }
}
</script>

<style scoped>
/* notice: 배경 이미지 이슈 해결 */
header {
  height: 1000px;
  background-size: 100% 100%;
  /* background-repeat: no-repeat;
  background-position: center;
  background-blend-mode: normal; */
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}
.subtitle__header {
  width: 520px;
  font-family: KaushanScript;
  font-size: 7.2rem;
  margin-top: 180px;
}
.title__header {
  width: 810px;
  font-family: Montserrat;
  font-size: 15rem;
  font-weight: bold;
  margin-top: 40px;
  margin-bottom: 70px;
}

.learn-more {
  width: 160px;
  height: 40px;
  font-family: Montserrat;
  font-size: 1.4rem;
  font-weight: bold;
  border: 3px solid #ffffff;
  margin-top: 50px;

  /* center */
  display: flex;
  justify-content: center;
  align-items: center;
}
.slides {
  display: flex;
  flex-grow: 1;
  align-items: flex-end;
  margin-bottom: 25px;
}
.slide {
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
.slide>.number {
  font-size: 2.4rem;
  font-weight: bold;
  padding-right: 5px;
}
</style>