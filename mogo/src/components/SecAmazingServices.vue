<template>
  <div class="amazing-services">
    <art-title></art-title>
    <div class="cards">
      <div class="card" v-for="card in cards" :key="card.title">
        <img class="card-icon" :src="`${require('@/images/amazing_services/' + card.icon + '.png')}`">
        <div>
          <div class="card-title">{{ card.title }}</div>
          <div class="card-content grey">{{ card.content }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ArtTitle from './ArtTitle'
export default {
  data() {
    return {
      cards:[
        {
          'icon': 'photography',
          'title': 'PHOTOGRAPHY',
          'content': 'LLorem ipsum dolor sit amet, consectetur adipiscing elit'
        },
        {
          'icon': 'web_design',
          'title': 'WEB DESIGN',
          'content': 'LLorem ipsum dolor sit amet, consectetur adipiscing elit'
        },
        {
          'icon': 'seo',
          'title': 'SEO',
          'content': 'LLorem ipsum dolor sit amet, consectetur adipiscing elit' 
        },
        
        {
          'icon': 'css_html',
          'title': 'CSS/HTML',
          'content': 'LLorem ipsum dolor sit amet, consectetur adipiscing elit'
        },
        {
          'icon': 'digital',
          'title': 'DIGITAL',
          'content': 'LLorem ipsum dolor sit amet, consectetur adipiscing elit'
        },
        {
          'icon': 'creativity',
          'title': 'CREATIVITY',
          'content': 'LLorem ipsum dolor sit amet, consectetur adipiscing elit'
        }
      ]
    }
  },
  components: {
    ArtTitle,
  }
}
</script>

<style scoped>
.amazing-services {
  text-align: center;
  position: relative;
  height: 650px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.cards {
  margin-top: 65px;
  display: flex;
  flex-wrap: wrap;
  padding: 0 20.3%;
}
.card{
  width: 33.33%;
  display: flex;
}
.card:nth-of-type(-n+3) {
  border-bottom: 1px solid #e5e5e5;
  margin-bottom: 47px;
}
.card-icon {
  width: 32px;
  height: 32px;
  margin-right: 27px;
}
.card-title{
  font-family: Montserrat;
  font-size: 1.4rem;
  text-align: left;
  font-weight: 500;
  color: #333333;
  margin-bottom: 10px;
}
.card-content {
  font-family: Roboto;
  font-size: 1.4rem;
  line-height: 1.6;
  text-align: left;
  padding-bottom: 50px;
}
</style>