<template>
  <div class="open-map" :style="{
    backgroundImage: `linear-gradient(to top, rgba(255,255,255,0.85), rgba(255,255,255,0.85)), url(${require('@/images/open_map_bg.png')})`}"
  >
    <img src="@/images/open_map_point.png" alt="" class="open-map-image">
    <span class="red">OPEN MAP</span>
    <hr class="underline bg-red">
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.open-map {
  padding-top: 57px;
  height: 200px;
  display: flex;
  flex-direction: column;
  justify-content: none;
  align-items: center;
}
.open-map-image {
  margin-bottom: 18px;
}
.open-map>span {
  font-family: Montserrat;
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 21px;
}
</style>