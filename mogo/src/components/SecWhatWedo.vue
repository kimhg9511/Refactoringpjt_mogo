<template>
  <div class="what-we-do">
    <art-title></art-title>
    <div class="comment grey">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua incididunt ut labore et dolore magna aliqua.</div>
    <div class="dropdowns">
      <img src="../images/what_we_do/what_we_do.png" alt="" class="floated-image">
      <div class="dropdown selected">
        <div class="drop-header">
          <img src="../images/what_we_do/photography.png" alt="" class="icon">
          <span class="header-title">PHOTOGRAPHY</span>
          <img src="../images/what_we_do/drop_up.png" class="toggle">
        </div>
        <div class="drop-body">
          <span class="drop-body-content">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
          </span>
        </div>
      </div>
    </div>
  <!-- <div class="dropdown">
    <div class="drop-header">
      <img src="../../static/mogo/img/mogo/mogo_wwd-creativity.png" alt="">
      <span class="header-title">CREATIVITY</span>
      <div class="toggle"><img src="../../static/mogo/img/mogo/mogo_drop-down.png" alt=""></div>
    </div>
    <div class="drop-body">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
    </div>
  </div>
  <div class="dropdown">
    <div class="drop-header">
      <img src="../../static/mogo/img/mogo/mogo_wwd-web-design.png" alt="">
      <span class="header-title">WEB DESIGN</span>
      <div class="toggle"><img src="../../static/mogo/img/mogo/mogo_drop-down.png" alt=""></div>
    </div>
    <div class="drop-body">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
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

<style scoped>
.what-we-do{
  height: 900px;  
}
.comment{
  padding-top: 270px;
  max-width: 950px;
  font-family: Roboto;
  font-size: 1.5rem;
  line-height: 1.6;
  text-align: center;

  margin: 0 auto 92px;
}
.dropdowns {
  display: flex;
  justify-content: center;
}
.floated-image {
  margin-right: 1.5625%;
}
.dropdown{
  margin-bottom: 10px;
}

.drop-header {
  width: 600px;
  height: 60px;
  border: solid 1px #e5e5e5;
  display: flex;

  align-items: center;  
}
.drop-header>.icon{
  margin-left: 16px;
  flex-grow: 0.5;
}
.drop-header>.header-title{
  font-family: Montserrat;
  font-weight: 500;
  font-size: 1.4rem;
  text-align: left;
  margin-left: 14px;
  flex-grow: 9;
}
.drop-header>.toggle {
  flex-grow: 0.5;
  margin-right: 20px;
}

.drop-body {
  width: 600px;
  height: 181px;
  border: solid 1px #e5e5e5;
  border-top: 0;
  position: relative;
}
.drop-body-content{
  height: 132px;
  font-family: Roboto;
  font-size: 15px;
  font-weight: 300;
  font-style: italic;
  line-height: 1.6;
  text-align: left;
  color: #999999;
  margin: 0;
  position: absolute;
  left: 0;
  padding-right: 28px;
  margin: 21px 25px 28px 20px;
  overflow-x : hidden;
  overflow-y : auto;
}
/* scroll css options */
.drop-body-content::-webkit-scrollbar{
  width: 5px;
}
.drop-body-content::-webkit-scrollbar-track{
  background-color: #f5f5f5;
}
.drop-body-content::-webkit-scrollbar-thumb{
  background-color: #95e1d3;
}
.drop-body-scroll {
  width: 5px;
  height: 140px;
  border-radius: 2.5px;
  background-color: #f38181;
  position: absolute;
  top:21px;
  right: 25px;
}
</style>