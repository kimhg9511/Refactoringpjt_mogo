<template>
  <div class="what-people-say">
    <art-title></art-title>
    <div class="cards">
      <div class="card" :key="client.name" v-for="client in clients">
        <div class="card-image">
          <img :src="`${require('../images/what_people_say/'+client.image+'.png')}`" alt="">
        </div>
        <div class="card-contents">
          <div class="contents-name">{{ client.name }}</div>
          <div class="contents-job">{{ client.job }}</div>
          <hr class="underline bg-red">
          <div class="contents-comment grey">
            {{ client.comment }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ArtTitle from './ArtTitle';

export default {
  components: {
    ArtTitle,
  },
  data() {
    return {
      clients: [
        {
          'image': 'matthew_dix',
          'name': 'MATTHEW DIX',
          'job': 'Graphic Design ',
          'comment': 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et.',
        },
        {
          'image': 'nick_karvounis',
          'name': 'Nick Karvounis',
          'job': 'Graphic Design',
          'comment': 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et.',
        },
        {
          'image': 'jaelynn_castillo',
          'name': 'Jaelynn Castillo',
          'job': 'Graphic Design',
          'comment': 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et.',
        },
        {
          'image': 'mike_petrucci',
          'name': 'Mike Petrucci',
          'job': 'Graphic Design',
          'comment': 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et.',
        }
      ]
    }
  }
}
</script>

<style>
/* notice: comment와의 세로 거리 맞출것. */
.what-people-say{
  height: 830px;
  background-image: linear-gradient(to top, rgba(255,255,255,0.85), rgba(255,255,255,0.85)), url('../images/what_people_say/bg.png');
  background-size: 100% 100%;
  padding: 0 18.8%;
}
.cards{
  margin-top: 87px;
  display: flex;
  flex-wrap: wrap;
}
.card{
  width: 50%;
  height: 200px;
  display: flex;
  padding: 0 40px;
}
.card:nth-of-type(-n+2) {
  margin-bottom: 80px;
}
.card-image {
  width: 110px;
  height: 110px;
  float: left;
}
.card-contents{
  margin-left: 30px;
  font-family: Roboto;
  font-size: 1.5rem;
}
.contents-name {
  font-family: Montserrat;
  font-weight: 500;
  font-size: 1.4rem;
  margin-bottom: 15px;
}
.contents-job {
  font-style: italic;
  margin-bottom: 17px;
}
.underline{
  margin-bottom: 27px;
}
.contents-comment {
  line-height: 1.6;
}
</style>