<template>
  <div class="sns-wrap bg-f8">
    <sec-sns></sec-sns>
    <sec-blogs></sec-blogs>
    <sec-instagram></sec-instagram>
  </div>
</template>

<script>
import SecSns from './SecSns';
import SecBlogs from './SecBlogs';
import SecInstagram from './SecInstagram';
export default {
  components: {
    SecSns,
    SecBlogs,
    SecInstagram,
  }
}
</script>

<style scoped>
.sns-wrap {
  width: 100%;
  height: 500px;
  padding: 70px 18.8%;
  /* padding: 70px 0; */
  display: flex;
  justify-content: center;
}
.sns-wrap>div:not(:last-of-type){
  margin-right: 30px;
}
</style>