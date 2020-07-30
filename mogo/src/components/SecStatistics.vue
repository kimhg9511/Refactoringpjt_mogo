<template>
  <div class="statistics bg-cyan">
    <div 
      class="item white"
      v-for="{number, name} in this.stats"
      :key = number
    >
      <p class="number">{{ number }}</p>
      <p class="name">{{ name }}</p>
    </div>
  </div>  
</template>

<style scoped>
.statistics{
  text-align: center;
  display: flex;
  justify-content: center;
  height: 270px;
}
.item{
  width: 240px;
  font-family: Montserrat;
  font-size: 1.4rem;
  border-left: 1px solid #ffffff;

  display: flex;
  flex-direction: column;
  justify-content: center;
}
.item:last-of-type{
  border-right: 1px solid #ffffff;
}

.number{
  height: 50px;
  line-height: 50px;
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

