<template>
  <div class="title-wrap">
    <span class="subtitle"><slot name="subtitle">subtitle</slot></span><br>
    <span class="title"><slot name="title">title</slot></span>
    <hr class="underline bg-red">
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.title-wrap{
  /* height: 200px; */
  position: relative;
}
.title-wrap>*{
  left: 50%;
  transform: translateX(-50%);
}
.subtitle {
  font-family: KaushanScript;
  font-size: 2.4rem;

  position: absolute;
  top:91px;
}
.title {
  font-family: Montserrat;
  font-size: 3rem;
  font-weight: bold;

  position: absolute;
  top: 137px;
}
.underline {
  width: 60px;
  height: 3px;
  border: 0;
  margin: 0;

  position: absolute;
  top: 200px;
}
</style>