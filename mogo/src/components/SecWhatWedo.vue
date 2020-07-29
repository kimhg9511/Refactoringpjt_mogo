<template>
  <div class="what-we-do">
    <art-title></art-title>
    <div class="comment grey">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua incididunt ut labore et dolore magna aliqua.</div>
    <div class="dropdown-wrap">
      <img src="../images/what_we_do/what_we_do.png" alt="" class="floated-image">
      <div class="dropdowns">
        <div class="dropdown" :key=item.title v-for="item in items">
          <div class="dropdown-header" @click="toggleDropdown(item)">
            <div class="header-icon">
              <img :src="`${require('@/images/amazing_services/' + item.icon + '.png')}`" alt="">
            </div>
            <span class="header-title">{{ item.title }}</span>
            <div class="header-toggle">
              <img src="../images/what_we_do/drop_up.png" v-if="item.selected">
              <img src="../images/what_we_do/drop_down.png" v-else>
            </div>
          </div>
          <div class="dropdown-body" v-if="item.selected">
            <span class="body-content grey">
              {{ item.contents }}
            </span>
          </div>
        </div>
      </div>
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
      items: [
        {
          'selected': true,
          'icon': 'photography',
          'title': 'PHOTOGRAPHY',
          'contents': 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.'
        },
        {
          'selected': false,
          'icon': 'creativity',
          'title': 'CREATIVITY',
          'contents': 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.'
        },
        {
          'selected': false,
          'icon': 'web_design',
          'title': 'WEB DESIGN',
          'contents': 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.'
        },
      ]
    }
  },
  methods: {
    toggleDropdown(item) {
      this.items.map(item => {
        if(item.selected) item.selected = !item.selected
      });
      item.selected = !item.selected;
    }
  }
}
</script>

<style scoped>
.what-we-do{
  height: 900px;  
  display: flex;
  flex-direction: column;
  align-items: center;
}
.comment{
  max-width: 950px;
  font-family: Roboto;
  font-size: 1.5rem;
  line-height: 1.6;
  text-align: center;

  margin: 42px 0 92px;
}
.dropdown-wrap {
  display: flex;
}
.floated-image {
  margin-right: 1.5625%;
}
.dropdown {
  margin-bottom: 10px;
}
.dropdown:last-of-type {
  margin: 0;
}
.dropdown-header {
  width: 600px;
  height: 60px;
  border: solid 1px #e5e5e5;
  display: flex;

  align-items: center;  
  justify-content: space-between;
}
.header-icon{
  margin-left: 16px;
}
.header-title{
  font-family: Montserrat;
  font-weight: 500;
  font-size: 1.4rem;
  margin-left: 14px;
  flex-grow: 1;
}
.header-toggle {
  margin-right: 20px;
}
.dropdown-body {
  width: 600px;
  height: 180px;
  border: solid 1px #e5e5e5;
  border-top: 0;
  position: relative;
}
.body-content{
  height: 140px;
  font-family: Roboto;
  font-size: 1.5rem;
  font-weight: 300;
  font-style: italic;
  line-height: 1.6;
  text-align: left;
  position: absolute;
  padding-right: 30px;
  margin: 20px 25px 0px 20px;
  overflow-x : hidden;
  overflow-y : auto;
}

/* scroll css options */
.body-content::-webkit-scrollbar{
  width: 5px;
}
.body-content::-webkit-scrollbar-track{
  background-color: #f5f5f5;
}
.body-content::-webkit-scrollbar-thumb{
  background-color: #95e1d3;
  border-radius: 2.5px;
}
</style>