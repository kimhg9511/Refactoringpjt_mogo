<template>
  <div class="statistics">
    <div 
      class="items white bg-cyan"
      v-for="{number, name} in this.stats"
      :key = number
    >
      <span class="number">{{number}}</span>
      <span class="name">{{name}}</span>
    </div>
  </div>  
</template>

<style scoped>
.statistics{
  text-align: center;
}
.items{
  width: 240px;
  height: 270px;
  font-family: Montserrat;
  font-size: 1.4rem;
  line-height: 1.4rem;
  border-left: 1px solid #ffffff;

  display: inline-block;
  position: relative;
}
.items:last-of-type{
  border-right: 1px solid #ffffff;
}
.number{
  height: 52px;
  line-height: 5.2rem;
  font-size: 7.2rem;
  font-weight: bold;

  position: absolute;
  top: 33.3333%;
  left: 50%;
  transform: translateX(-50%);
}
.name{
  position: absolute;
  bottom: 33.3333%;
  left: 50%;
  transform: translateX(-50%);
}
</style>

<script>
export default {
  data() {
    return {
      stats: [
        {
          'number': 42,
          'name': 'WEB DESIGN PROJECTS'
        },
        {
          'number': 123,
          'name': 'HAPPY CLIENT'
        },
        {
          'number': 15,
          'name': 'AWARD WINNER'
        },
        {
          'number': 99,
          'name': 'CUP OF COFFEE'
        },
        {
          'number': 24,
          'name': 'MEMBERS'
        }  
      ]
    }
  }
}
</script>

