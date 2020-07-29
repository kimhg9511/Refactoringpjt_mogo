<template>
  <div class='nav-bar'>
    <div class="logo">MoGo</div>
    <div class="nav-items">
      <div class="nav-item" :key="navItem" v-for="navItem in navItems">
        <img :src="`${require('@/images/header/'+navItem+'.png')}`" alt="" v-if="navItem=='cart' || navItem=='search'">
        <span v-else>
          {{ navItem }}
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navItems: [
        'ABOUT',
        'SERVICE',
        'WORK',
        'BLOG',
        'CONTACT',
        'cart',
        'search'
      ]
    }
  }
}
</script>

<style scoped>
.nav-bar {
  width: 100%;
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
  text-align: left;
  flex-basis: auto;
  height: 50px;
}
.logo {
  font-family: Montserrat;
  font-size: 3rem;
  font-weight: bold;
  margin-left: 18.8%;
}
.nav-items{
  width: 620px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-right: 18.8%;
}
.nav-item>span{
  font-family: Montserrat;
  font-size: 1.4rem;
}
.nav-item:nth-of-type(-n+5){
  flex-grow: 1;
}
.nav-item:nth-of-type(6){
  flex-grow: 0.8;
}
</style>