<template>
  <div class="title">
    <span class="sub-title"><slot name="subtitle">subtitle</slot></span><br>
    <span class="main-title"><slot name="title">title</slot></span>
    <hr class="underline bg-red">
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.title{
  height: 200px;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
}
.sub-title {
  font-family: KaushanScript;
  font-size: 2.4rem;
}
.main-title {
  font-family: Montserrat;
  font-size: 3rem;
  font-weight: bold;
  margin-top: 23px;
}
.underline {
  width: 60px;
  height: 3px;
  border: none;
  margin: 40px 0 0;
}
</style>