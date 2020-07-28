<template>
  <div class="statistics bg-cyan">
    <div 
      class="items white"
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
  display: flex;
  justify-content: center;
}
.items{
  width: 240px;
  height: 270px;
  font-family: Montserrat;
  font-size: 1.4rem;
  line-height: 1.4rem;
  border-left: 1px solid #ffffff;

  display: flex;
  flex-direction: column;
}
.items:last-of-type{
  border-right: 1px solid #ffffff;
}
.number{
  height: 50px;
  line-height: 50px;
  margin-top: 33%;
  font-size: 7.2rem;
  font-weight: bold;
  margin-bottom: 30px;
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

