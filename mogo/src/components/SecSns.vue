<template>
  <div class="panel sns">
    <span class="mogo">MoGo</span><br>
    <span class="contents grey">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation.</span><br>
    <span class="followers"><span class="followers-number">15k </span>followers</span>
    <div class="sns-image-wrap">
      <span class="follow-us grey">Follow Us: </span>
      <div class="sns-image"><img src="../images/sns/sns_1.png" alt=""></div>
      <div class="sns-image"><img src="../images/sns/sns_2.png" alt=""></div>
      <div class="sns-image"><img src="../images/sns/sns_3.png" alt=""></div>
      <div class="sns-image"><img src="../images/sns/sns_4.png" alt=""></div>
      <div class="sns-image"><img src="../images/sns/sns_5.png" alt=""></div>
      <div class="sns-image"><img src="../images/sns/sns_6.png" alt=""></div>
      <div class="sns-image"><img src="../images/sns/sns_7.png" alt=""></div>
      <div class="sns-image"><img src="../images/sns/sns_8.png" alt=""></div>
    </div>
    <form action="#">
      <input type="text" placeholder="Your Email" class="email-input">
      <input type="button" class="subscribe-button white bg-cyan" value="SUBSCRIBE">
    </form>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.sns{
  width: 480px;
  flex-shrink: 0;
  display: flex;
  flex-direction: column;
}
.mogo {
  font-family: Montserrat;
  font-size: 4.65rem;
  font-weight: bold;
  color: #cccccc;
  margin-bottom: 42px;
}
.contents {
  font-size: 1.5rem;
  line-height: 1.6;
  margin-bottom: 40px;
}
.followers {
  font-family: Montserrat;
  font-size: 1.4rem;
  padding-bottom: 18px;
  border-bottom: 1px solid #e5e5e5;
  margin-bottom: 18px;
}
.followers-number {
  font-size: 18px;
  font-weight: bold;
}
.sns-image-wrap{
  display: flex;
  justify-content: flex-start;
  margin-bottom: 40px;
}
.follow-us {
  width: 70px;
  font-size: 1.5rem;
  font-weight: 300;
  font-style: italic;
}
.sns-image-wrap> * {
  margin-right: 15px;
}
.email-input {
  width: 50%;
  height: 40px;
  border: solid 1px #e7e7e7;
}
.email-input::placeholder{
  font-size: 1.5rem;
  font-weight: 300;
  font-style: italic;
  color: #cccccc;
  position: relative;
  left: 13px;
}
.subscribe-button {
  width: 33%;
  height: 40px;
  border: solid 1px #e7e7e7;
  font-family: Montserrat;
  font-size: 1.4rem;
  font-weight: 500;
}
</style>