<template>
  <div class="unique-design">
    <art-title></art-title>
    <div class="main" >
      <div class="attached"></div>
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
.unique-design {
  height: 850px;
  background-image: linear-gradient(to top, rgba(255,255,255,0.85), rgba(255,255,255,0.85)), url('../images/unique_design/bg.png');
  position: relative;
}
.main {
  width: 570px;
  height: 620px;
  position: absolute;
  bottom: 0;
  left: 48.5%;
  transform: translateX(-50%);
  background-image: url("../images/unique_design/main.png");
}
.attached {
  width: 275px;
  height: 475px;
  position: absolute;
  bottom: -15.2%;
  right: 0;
  transform: translateX(42%);
  background-image: url("../images/unique_design/attached.png");
}
</style>