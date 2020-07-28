<template>
  <div class="latest-blog">
    <art-title></art-title>
    <div class="blog-cards">
      <div class="blog-card" :key="post.name" v-for="post in posts">
        <div class="card-image">
          <img :src="`${require('../images/latest_blog/'+post.image+'.png')}`" alt="">
          <div class="image-attach bg-cyan">
            <span class="attach-month white">
              {{ post.date }}
            </span>
            <span class="attach-day white">
              Jan
            </span>
          </div>
        </div>
        <div class="card-title">{{ post.title }}</div>
        <span class="card-description grey">
          {{ post.description }}
        </span>
        <div class="reply-wrap">
          <img src="../images/latest_blog/view.png" alt="">
          <span class="reply-count grey">{{ post.viewCnt }}</span>
          <img src="../images/latest_blog/comment.png" alt="">
          <span class="reply-count grey">{{ post.commentCnt }}</span>
        </div>
      </div>
      <!-- <div class="blog-card">
        <div class="card-image">
            <div class="image-attach">
              <span class="attach-month">
                14
                <span class="attach-day">
                  Jan
                </span>
              </span>
            </div>
        </div>
        <div class="card-title">Lorem ipsum dolor sit amet</div>
        <span class="card-description">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit
        </span>
        <hr>
        <div class="reply-wrap">
          <div class="repl-image one"></div><span class="reply-count">992</span>
          <div class="repl-image two"></div><span class="reply-count">42</span>
        </div>
      </div>
      <div class="blog-card">
        <div class="card-image">
          <div class="image-attach">
            <span class="attach-month">
              15
              <span class="attach-day">
                Jan
              </span>
            </span>
          </div>
        </div>
        <div class="card-title">Lorem ipsum dolor sit amet</div>
        <span class="card-description">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit
        </span>
        <hr>
        <div class="reply-wrap">
          <div class="repl-image one"></div><span class="reply-count">1550</span>
          <div class="repl-image two"></div><span class="reply-count">98</span>
        </div>
      </div> -->
    </div>
  </div>
</template>

<script>
import ArtTitle from '../components/ArtTitle'
export default {
  components: {
    ArtTitle,
  },
  data() {
    return {
      posts: [
        {
          image:'1',
          name:'a',
          date:'15',
          title:'Lorem ipsum dolor sit amet',
          description:'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
          viewCnt: 542,
          commentCnt: 77,
        }
      ]
    }
  }
}
</script>

<style scoped>
.latest-blog{
  height: 770px;
}
.blog-cards{
  display: flex;
  padding: 47px 18.8% 0;
}
.blog-card{
  width: 33%;
  display: flex;
  flex-direction: column;
}
.card-image {
  width: 100%;
  position: relative;
  margin: 0 0 20px;
}
.card-image>img{
  width: 100%;
  height: 100%;
}
.image-attach{
  width: 60px;
  height: 70px;
  text-align: center;
  position: absolute;
  bottom: 10px;
  left: -10px;

  /* 하위 요소 flex */
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.attach-month {
  font-family: Montserrat;
  font-size: 3rem;
  font-weight: bold;
}
.attach-day {
  font-size: 1.5rem;
  font-style: italic;
}
.card-title {
  font-family: Montserrat;
  font-size: 1.4rem;
  margin-bottom: 20px;
}
.card-description{
  font-size: 1.5rem;
  line-height: 1.6;
  padding-bottom: 20px;
  border-bottom: 1px solid #e5e5e5;
  margin-bottom: 20px;
}
.reply-wrap {
  display: flex;
}
.reply-count{
  font-style: italic;
  margin-left: 6px;
  margin-right: 18px;
}
</style>