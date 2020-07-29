<template>
  <div class="meet-our-team">
    <art-title></art-title>
    <span class="comment grey">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</span>
    <div class="cards">
      <div class="card" :key="card.name" v-for="card in cards" @click="card.selected = !card.selected">
        <div class="card-image bg-cyan">
          <img :src="`${require('../images/meet_our_team/'+card.image+'.png')}`" alt="">
          <div class="card-menu" v-if="card.selected">
            <div class="menu-item bg-yellow">
              
            </div>
            <div class="menu-item bg-yellow">

            </div>
            <div class="menu-item bg-yellow">

            </div>
            <div class="menu-item bg-yellow">

            </div>
          </div>
        </div>
        <div class="card-name">{{ card.name }}</div><br>
        <div class="card-job grey">{{ card.job }}</div>
      </div>
    </div>
    <div class="logos bg-f8">
      <img src="../images/meet_our_team/logos.png" alt="">
    </div>
  </div>  
</template>

<script>
import ArtTitle from './ArtTitle'
export default {
  components: {
    ArtTitle,
  },
  data() {
    return {
      cards: [
        {
          'selected': false,
          'image': 'matthew_dix',
          'name': 'MATTHEW DIX',
          'job': 'Graphic Design',
        },
        {
          'selected': false,
          'image': 'christopher_campbell',
          'name': 'CHRISTOPHER CAMPBELL',
          'job': 'Branding/UX design',
        },
        {
          'selected': false,
          'image': 'michael_fertig',
          'name': 'MICHAEL FERTIG',
          'job': 'Developer',
        },
      ]
    }
  }
}
</script>

<style scoped>
.meet-our-team{
  height: 1290px;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: start;
}
.comment {
  width: 954px;
  height: 39px;
  font-family: Roboto;
  font-size: 1.5rem;
  line-height: 1.6;
  margin: 46px 0 92px;
}
.cards {
  display: flex;
  margin-bottom: 117px;
}
.card {
  margin: 0 15px;
}
.card-image {
  width: 380px;
  height: 470px;
  margin-bottom: 31px;
  position: relative;
}
.card-menu{
  width: 228px;
  height: 56px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.menu-item {
  display: inline-block;
  width: 56px;
  height: 56px;
  margin: 0;
}
.menu-item:not(:last-of-type){
  border-right: 1px solid #f38181;
}
.card-name {
  font-family: Montserrat;
  font-weight: 500;
  font-size: 1.4rem;
  text-align: center;
  margin-bottom: 5px;
}
.card-job {
  font-family: Roboto;
  font-size: 1.5rem;
  font-weight: 300;
  font-style: italic;
}
.logos {
  width: 100%;
  height: 250px;
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>