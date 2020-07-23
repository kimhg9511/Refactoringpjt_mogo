<template>
  <div class="amazing-services">
    <span class="subtitle">We work with</span><br>
    <span class="title">AMAZING SERVICES</span>
    <hr class="underline bg-red">
    <div class="items">
      <span class="services-title">PHOTOGRAPHY</span><br>
      <span class="services-content">LLorem ipsum dolor sit amet, consectetur adipiscing elit</span>
    </div>
  </div>
</template>
PHOTOGRAPHY
WEB DESIGN
CREATIVITY
SEO
CSS/HTML
DIGITAL
LLorem ipsum dolor sit amet, consectetur adipiscing elit
<style scoped>
/* section we-work-with */
.amazing-services{
  text-align: center;
  position: relative;
  height: 650px;
}
/* .weworkwith>*{
  left: 50%;
  transform: translateX(-50%);
} */

.items{
    width: 333px;
    height: 120px;
    height: 70px;
    margin: 0 34px;
    display: inline-block;
}
.items>img{ 
    width: 32px;
    height: 32px;
    float: left;
}
.services-title{
    height: 10px;
    font-family: Montserrat;
    font-size: 14px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: normal;
    letter-spacing: normal;
    text-align: left;
    color: #333333;
    /**/
    /* line-height: 10px; */
    float: left;
    margin-left: 27px;
    /* margin-bottom: 20px; */
}
.services-content {
    width: 300px;
    height: 39px;
    font-family: Roboto;
    font-size: 15px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.6;
    letter-spacing: normal;
    text-align: left;
    color: #999999;
    margin-left: 59px;
    margin-top: -2px;
  }
/* end of section we-work-with */
</style>

<script>
export default {
  data() {
    return {
      cards:{
        'title': [

        ],
        'content': [

        ]
      }
    }
  }
}
</script>
