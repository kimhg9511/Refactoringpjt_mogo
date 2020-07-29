<template>
   <div class="blogs">
    <div class="blogs-title">BLOGS</div>
    <div class="blogs-item" :key="post.image" v-for="post in posts">
      <img :src="`${require('../images/sns/blogs_'+post.image+'.png')}`" alt="">
      <div class="item-summary">
        <p class="summary-title">
          {{ post.title }}
        </p>
        <p class="summary-date grey">
          {{ post.date }}
        </p>
      </div>
    </div>
  </div>  
</template>

<script>
export default {
  data() {
    return {
      posts: [
        {
          image:'1',
          title:'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
          date: 'Jan 9, 2016',
        },
                {
          image:'2',
          title:'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
          date: 'Jan 9, 2016',
        },
                {
          image:'3',
          title:'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
          date: 'Jan 9, 2016',
        }
      ]
    }
  }
}
</script>

<style scoped>
.blogs{
  flex-shrink: 0;
  width: 360px;
}
.blogs-title {
  font-family: Montserrat;
  font-size: 1.4rem;
  font-weight: 500;
  margin-bottom: 40px;
}
.blogs-item{
  width: 100%;
  margin-bottom: 30px;
  display: flex;
  align-items: flex-end;
}
.blogs-item>.item-summary{
  margin-left: 20px;
}
.summary-title {
  font-family: Montserrat;
  font-size: 1.2rem;
  line-height: 1.5;
  font-weight: 500;
  margin-bottom: 5px;
}
.summary-date {
  font-weight: 300;
  font-size: 1.3rem;
  font-style: italic;
  margin-bottom: 5px;
}
</style>